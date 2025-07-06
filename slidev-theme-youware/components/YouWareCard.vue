<template>
  <div class="yw-card">
    <h3 v-if="title" class="card-title">{{ title }}</h3>
    <div class="card-content">
      <slot />
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  title?: string
}>()
</script>

<style scoped>
.yw-card {
  background-color: var(--yw-bg-white);
  border: 1px solid var(--yw-border);
  border-radius: 12px;
  padding: 2rem;
  box-shadow: var(--yw-shadow-sm);
  transition: box-shadow 0.2s ease;
  margin: 1rem 0;
}

.yw-card:hover {
  box-shadow: var(--yw-shadow-md);
}

.card-title {
  margin-top: 0;
  margin-bottom: 1rem;
  color: var(--yw-text-primary);
}

.card-content {
  color: var(--yw-text-secondary);
}
</style>