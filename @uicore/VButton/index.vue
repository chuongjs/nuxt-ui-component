<template>
  <component v-bind="attributes" :class="classes">
    <div class="v-button__content">
      <slot></slot>
    </div>
  </component>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
interface AnyObject {
  [key: string]: any
}
export default defineComponent({
  name: 'VButton',
  props: {
    type: {
      type: String,
      default: '', // primary / success / warning / danger / info / text
    },
    nativeType: {
      type: String,
      default: '', // button / submit / reset
    },
    size: {
      type: String,
      default: '', // medium / small / mini
    },
    width: {
      type: String,
      default: '',
    },
    height: {
      type: String,
      default: '',
    },
    plain: {
      type: Boolean,
      default: false,
    },
    round: {
      type: Boolean,
      default: false,
    },
    circle: {
      type: Boolean,
      default: false,
    },
    loading: {
      type: Boolean,
      default: false,
    },
    disabled: {
      type: Boolean,
      default: false,
    },
    to: {
      type: String,
      default: '',
    },
  },
  data() {
    return {
      execute: ['size', 'plain', 'round', 'circle', 'loading'],
    }
  },
  computed: {
    component(): string {
      return this.$props.to && !this.$props.disabled ? 'router-link' : 'button'
    },
    classes(): string {
      const classList: string[] = ['v-button']
      const { disabled, to, plain } = this.$props
      if (disabled) classList.push('is-disabled')
      if (to) classList.push(`v-button__link`)
      Object.entries(this.$props).forEach(([key, value]) => {
        const isHasBeen = this.execute.includes(key)
        if (isHasBeen && typeof value === 'boolean' && value) {
          classList.push(`is-${key}`)
        } else if (isHasBeen && key === 'size' && value) {
          classList.push(`v-button--${value}`)
        } else if (key === 'type') {
          value = plain && value === 'dark' ? '' : value
          classList.push(`v-button--${value || 'default'}`)
        }
      })
      return classList.join(' ')
    },
    attributes(): AnyObject {
      const attrs: AnyObject = {
        is: this.component,
      }
      const styles: string[] = []
      Object.entries(this.$props).forEach(([key, value]) => {
        const isHasBeen = this.execute.includes(key)
        if (key !== 'to' && key === 'nativeType') {
          attrs['type'] = value || 'button'
        } else if (key === 'height' && value) {
          styles.push([key, value].join(':'))
        } else if (key === 'width' && value) {
          styles.push([key, value].join(':'))
        } else if (!isHasBeen && value) {
          attrs[key] = value
        }
      })
      attrs['style'] = styles.join(';')
      return attrs
    },
  },
  mounted() {},
  methods: {},
})
</script>

<style lang="sass" scoped>
@import './v-button'
</style>
