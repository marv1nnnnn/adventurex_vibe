<template>
  <div class="slidev-layout cover" style="background-color: var(--slidev-theme-primary-bg);">
    <div class="my-auto w-full max-w-4xl mx-auto px-8 text-center">
      <slot />
    </div>
  </div>
</template>

<style scoped>
.cover {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
