<template>
  <div class="slidev-layout intro" style="background-color: var(--slidev-theme-primary-bg);">
    <div class="my-auto max-w-5xl mx-auto px-12">
      <slot />
    </div>
  </div>
</template>

<style scoped>
.intro {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
