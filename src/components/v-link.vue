<template>
    <div href="/" class="like-link">
        <slot />
    </div>
</template>

<style scoped>
.like-link {
    color: #1867c0;
    min-width: 64px;
    padding: 0 16px;
}

.like-link:hover {
    opacity: 0.5;
}
</style>