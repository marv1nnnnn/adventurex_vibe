<template>
  <div class="slidev-layout cover">
    <div class="yw-logo" v-if="$slidev.configs.logo">
      <img :src="$slidev.configs.logo" alt="Logo" />
    </div>
    
    <div class="cover-content">
      <slot />
    </div>
    
    <div class="cover-footer" v-if="$slidev.configs.event || $slidev.configs.date">
      <span v-if="$slidev.configs.event" class="yw-tag">{{ $slidev.configs.event }}</span>
      <span v-if="$slidev.configs.date" class="cover-date">{{ $slidev.configs.date }}</span>
    </div>
  </div>
</template>

<style scoped>
.yw-logo {
  position: absolute;
  top: 3rem;
  left: 3rem;
}

.yw-logo img {
  height: 2rem;
}

.cover-content {
  max-width: 900px;
  margin: 0 auto;
  padding: 4rem;
}

.cover-footer {
  position: absolute;
  bottom: 3rem;
  left: 50%;
  transform: translateX(-50%);
  display: flex;
  align-items: center;
  gap: 1.5rem;
}

.cover-date {
  color: var(--yw-text-secondary);
  font-size: 1rem;
}
</style>