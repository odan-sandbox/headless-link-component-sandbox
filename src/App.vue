<template>
  <div class="links">
    <VLink class="v-link" type="underlined-link">
      <VHeadlessLink> poyo </VHeadlessLink>
    </VLink>
    <VLink class="v-link" type="link-primary">
      <VHeadlessLink> poyo </VHeadlessLink>
    </VLink>
    <VLink class="v-link" type="button">
      <VHeadlessLink> poyo </VHeadlessLink>
    </VLink>
  </div>
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

<style scoped>
.links {
  display: flex;
  flex-direction: column;
}

.v-link {
  margin: 8px 0px;
  display: flex;
  align-content: center;
  justify-content: center;
  flex: 1 1 auto;
}
</style>
