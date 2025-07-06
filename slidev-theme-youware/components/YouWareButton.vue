<template>
  <component
    :is="tag"
    :href="href"
    :to="to"
    class="yw-button"
    :class="[variant]"
  >
    <slot />
  </component>
</template>

<script setup lang="ts">
import { computed } from 'vue'

const props = defineProps<{
  href?: string
  to?: string
  variant?: 'primary' | 'secondary'
}>()

const tag = computed(() => {
  if (props.href) return 'a'
  if (props.to) return 'RouterLink'
  return 'button'
})
</script>

<style scoped>
.yw-button {
  display: inline-block;
  padding: 0.75rem 2rem;
  background-color: var(--yw-accent-green);
  color: white;
  border: 2px solid transparent;
  border-radius: 8px;
  font-weight: 500;
  text-decoration: none;
  transition: all 0.2s ease;
  box-shadow: var(--yw-shadow-sm);
  cursor: pointer;
  font-size: 1rem;
}

.yw-button:hover {
  background-color: var(--yw-accent-green-hover);
  transform: translateY(-1px);
  box-shadow: var(--yw-shadow-md);
}

.yw-button.secondary {
  background-color: transparent;
  color: var(--yw-accent-green);
  border-color: var(--yw-accent-green);
}

.yw-button.secondary:hover {
  background-color: var(--yw-accent-green);
  color: white;
}
</style>