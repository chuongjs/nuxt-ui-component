<template>
  <svg
    width="7"
    height="12"
    viewBox="0 0 7 12"
    fill="none"
    xmlns="http://www.w3.org/2000/svg"
  >
    <path
      d="M5.1875 11.2812L0.71875 6.53125C0.59375 6.375 0.5 6.1875 0.5 6C0.5 5.84375 0.59375 5.65625 0.71875 5.5L5.1875 0.75C5.46875 0.4375 5.9375 0.4375 6.25 0.71875C6.5625 1 6.5625 1.46875 6.28125 1.78125L2.25 6.03125L6.28125 10.25C6.5625 10.5625 6.5625 11.0312 6.25 11.3125C5.9375 11.5938 5.46875 11.5938 5.1875 11.2812Z"
      :fill="color"
    />
  </svg>
</template>

<script lang="ts">
export default {
  name: 'IconChervonLeft',
  props: {
    color: {
      type: String,
      default: '#303439',
    },
  },
}
</script>
