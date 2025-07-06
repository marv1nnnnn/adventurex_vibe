<template>
  <div class="slidev-layout two-cols" :class="props.class">
    <div class="col-left">
      <slot />
    </div>
    <div class="col-right">
      <slot name="right" />
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  class?: string
}>()
</script>

<style scoped>
.col-left,
.col-right {
  height: 100%;
}
</style>