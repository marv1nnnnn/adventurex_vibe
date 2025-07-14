<template>
  <div class="youware-card" :class="{ 'hoverable': hoverable }">
    <slot />
  </div>
</template>

<script setup lang="ts">
interface Props {
  hoverable?: boolean
}

withDefaults(defineProps<Props>(), {
  hoverable: false,
})
</script>

<style scoped>
.youware-card {
  background-color: var(--slidev-theme-card-bg);
  border: 1px solid var(--slidev-theme-border-color);
  border-radius: 8px;
  padding: 24px;
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.04);
  transition: all 0.3s ease;
}

.youware-card.hoverable:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.08);
  border-color: var(--slidev-theme-accent-green);
}
</style>