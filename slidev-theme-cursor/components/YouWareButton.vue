<template>
  <button
    class="youware-button"
    :class="[size, { 'full-width': fullWidth }]"
    @click="$emit('click')"
  >
    <slot />
  </button>
</template>

<script setup lang="ts">
interface Props {
  size?: 'small' | 'medium' | 'large'
  fullWidth?: boolean
}

withDefaults(defineProps<Props>(), {
  size: 'medium',
  fullWidth: false,
})

defineEmits<{
  click: []
}>()
</script>

<style scoped>
.youware-button {
  background-color: var(--slidev-theme-accent-green);
  color: white;
  border: none;
  border-radius: 24px;
  font-family: var(--slidev-font-primary);
  font-weight: 500;
  cursor: pointer;
  transition: all 0.2s ease;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  letter-spacing: 0.02em;
}

.youware-button:hover {
  background-color: #4A5640;
  transform: translateY(-1px);
  box-shadow: 0 4px 12px rgba(90, 102, 80, 0.2);
}

.youware-button:active {
  transform: translateY(0);
  box-shadow: 0 2px 6px rgba(90, 102, 80, 0.2);
}

/* Sizes */
.small {
  padding: 8px 20px;
  font-size: 14px;
}

.medium {
  padding: 12px 32px;
  font-size: 16px;
}

.large {
  padding: 16px 48px;
  font-size: 18px;
}

.full-width {
  width: 100%;
}
</style>