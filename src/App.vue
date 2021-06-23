<template>
  <VLink>
    <VHeadlessLink />
  </VLink>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import VLink from "./components/v-link.vue";
import VHeadlessLink from "./components/v-headless-link.vue";

export default defineComponent({
  name: "App",
  components: {
    VLink,
    VHeadlessLink,
  },
});
</script>

<style>
#app {
  text-align: center;
  margin-top: 60px;
}
:root {
  --color-text-link: rgb(3, 102, 214);
  --color-text-primary: rgb(36, 41, 46);
}
</style>
