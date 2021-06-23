<template>
  <div href="/" class="like-link">
    <slot />
  </div>
</template>

<style scoped>
.like-link {
  color: var(--color-text-primary);
  min-width: 64px;
  padding: 0 16px;
}

.like-link:hover {
  color: var(--color-text-link);
}
</style>
