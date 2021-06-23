<template>
  <div
    href="/"
    class="v-link"
    :class="{
      'underlined-link': underlinedLink,
      'link-primary': linkPrimary,
      button,
    }"
  >
    <slot />
  </div>
</template>

<script lang="ts">
import { defineComponent, PropType } from "vue";

export type Type = "underlined-link" | "link-primary" | "button";

export default defineComponent({
  props: {
    type: {
      type: String as PropType<Type>,
      required: true,
    },
  },
  setup(props) {
    return {
      underlinedLink: props.type === "underlined-link",
      linkPrimary: props.type === "link-primary",
      button: props.type === "button",
    };
  },
});
</script>

<style scoped>
.v-link {
  display: inline-block;
}

.underlined-link {
  color: var(--color-text-link);
  font-weight: 700;
}

.underlined-link:hover {
  text-decoration: underline;
}

.link-primary {
  color: var(--color-text-primary);
  font-weight: 700;
}

.link-primary:hover {
  color: var(--color-text-link);
}

.button {
  padding: 12px 3px;
  border: 1px solid;
  border-radius: 6px;
  background-color: #fafbfc;
  box-shadow: rgba(27, 31, 35, 0.04) 0px 1px 0px 0px,
    rgba(255, 255, 255, 0.25) 0px 1px 0px 0px inset;
}
</style>
