<template>
  <VLink>
    <VHeadlessLink />
  </VLink>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import VLink from './components/v-link.vue'
import VHeadlessLink from './components/v-headless-link.vue'

export default defineComponent({
  name: 'App',
  components: {
    VLink,
    VHeadlessLink
  }
})
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
