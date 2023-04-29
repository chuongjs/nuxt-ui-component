<template>
  <div>
    <div>
      <v-button to="/"> Về trang chủ </v-button>
      <v-button to="/" round type="primary">
        <icon-chervon-left color="white" />
        Về trang chủ
      </v-button>
      <v-button to="/" circle type="dark">
        <icon-chervon-left color="white" />
      </v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button to="/" size="small" type="warning"> Về trang chủ </v-button>
      <v-button to="/" size="small" type="danger" round>
        <icon-chervon-left color="white" />
        Về trang chủ
      </v-button>
      <v-button to="/" size="small" type="success" circle>
        <icon-chervon-left color="white" />
      </v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button to="/" size="mini"> Về trang chủ </v-button>
      <v-button to="/" size="mini" round>
        <icon-chervon-left />
        Về trang chủ
      </v-button>
      <v-button to="/" size="mini" circle>
        <icon-chervon-left />
      </v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button>Default</v-button>
      <v-button size="small">Small</v-button>
      <v-button size="mini">Mini</v-button>
      <v-button size="small" circle>1</v-button>
      <v-button to="/" round size="small">Link</v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button disabled>Default</v-button>
      <v-button size="small" disabled>Small</v-button>
      <v-button size="mini" disabled>Mini</v-button>
      <v-button size="small" circle disabled>1</v-button>
      <v-button to="/" round size="small" disabled>Link</v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button size="small" round>First</v-button>
      <v-button size="small" round>Previous</v-button>
      <v-button size="small" type="primary" round>1</v-button>
      <v-button size="small" round>2</v-button>
      <v-button size="small" round>...</v-button>
      <v-button size="small" round>120</v-button>
      <v-button size="small" round>121</v-button>
      <v-button size="small" round>Next</v-button>
      <v-button size="small" round>Last</v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button type="dark">Default</v-button>
      <v-button type="dark" size="small">Small</v-button>
      <v-button type="dark" size="mini">Mini</v-button>
      <v-button type="dark" size="small" circle>5</v-button>
      <v-button type="dark" to="/" round size="small"> Link </v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button type="dark" disabled>Default</v-button>
      <v-button type="dark" size="small" disabled>Small</v-button>
      <v-button type="dark" size="mini" disabled>Mini</v-button>
      <v-button type="dark" size="small" circle disabled>5</v-button>
      <v-button type="dark" to="/" round size="small" disabled> Link </v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button type="primary">Default</v-button>
      <v-button type="primary" size="small">Small</v-button>
      <v-button type="primary" size="mini">Mini</v-button>
      <v-button type="primary" size="small" circle>2</v-button>
      <v-button type="primary" to="/" round size="small"> Link </v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button type="primary" disabled>Default</v-button>
      <v-button type="primary" size="small" disabled>Small</v-button>
      <v-button type="primary" size="mini" disabled>Mini</v-button>
      <v-button type="primary" size="small" circle disabled>2</v-button>
      <v-button type="primary" to="/" round size="small" disabled>
        Link
      </v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button type="warning">Default</v-button>
      <v-button type="warning" size="small">Small</v-button>
      <v-button type="warning" size="mini">Mini</v-button>
      <v-button type="warning" size="small" circle>3</v-button>
      <v-button type="warning" to="/" round size="small"> Link </v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button type="warning" disabled>Default</v-button>
      <v-button type="warning" size="small" disabled>Small</v-button>
      <v-button type="warning" size="mini" disabled>Mini</v-button>
      <v-button type="warning" size="small" circle disabled>3</v-button>
      <v-button type="warning" to="/" round size="small" disabled>
        Link
      </v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button type="success">Default</v-button>
      <v-button type="success" size="small">Small</v-button>
      <v-button type="success" size="mini">Mini</v-button>
      <v-button type="success" size="small" circle>4</v-button>
      <v-button type="success" to="/" round size="small"> Link </v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button type="success" disabled>Default</v-button>
      <v-button type="success" size="small" disabled>Small</v-button>
      <v-button type="success" size="mini" disabled>Mini</v-button>
      <v-button type="success" size="small" circle disabled>4</v-button>
      <v-button type="success" to="/" round size="small" disabled>
        Link
      </v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button type="danger">Default</v-button>
      <v-button type="danger" size="small">Small</v-button>
      <v-button type="danger" size="mini">Mini</v-button>
      <v-button type="danger" size="small" circle>5</v-button>
      <v-button type="danger" to="/" round size="small"> Link </v-button>
    </div>

    <div style="margin-top: 1rem">
      <v-button type="danger" disabled>Default</v-button>
      <v-button type="danger" size="small" disabled>Small</v-button>
      <v-button type="danger" size="mini" disabled>Mini</v-button>
      <v-button type="danger" size="small" circle disabled>5</v-button>
      <v-button type="danger" to="/" round size="small" disabled>
        Link
      </v-button>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'ButtonPage',
})
</script>
