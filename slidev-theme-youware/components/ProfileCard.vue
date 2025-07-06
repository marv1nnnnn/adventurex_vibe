<template>
  <div class="profile-card">
    <div class="profile-header">
      <div class="profile-avatar" v-if="avatar">
        <img :src="avatar" :alt="name" />
      </div>
      <div class="profile-info">
        <h3 class="profile-name">{{ name }}</h3>
        <p class="profile-title" v-if="title">{{ title }}</p>
      </div>
    </div>
    <div class="profile-content" v-if="$slots.default">
      <slot />
    </div>
    <div class="profile-items" v-if="items && items.length">
      <div class="profile-item" v-for="(item, index) in items" :key="index">
        <span class="item-icon">{{ item.icon || '•' }}</span>
        <span class="item-text">{{ item.text }}</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
interface ProfileItem {
  icon?: string
  text: string
}

defineProps<{
  name: string
  title?: string
  avatar?: string
  items?: ProfileItem[]
}>()
</script>

<style scoped>
.profile-card {
  background: rgba(255, 255, 255, 0.95);
  backdrop-filter: blur(10px);
  border: 1px solid var(--yw-border);
  border-radius: 16px;
  padding: 2rem;
  box-shadow: 0 8px 24px rgba(45, 45, 45, 0.08);
  max-width: 700px;
  margin: 1.5rem auto;
  animation: slideUp 0.8s ease-out;
}

.profile-header {
  display: flex;
  align-items: center;
  gap: 1.5rem;
  margin-bottom: 1.5rem;
}

.profile-avatar {
  width: 80px;
  height: 80px;
  border-radius: 50%;
  overflow: hidden;
  border: 3px solid var(--yw-accent-green);
  box-shadow: 0 4px 12px rgba(74, 103, 65, 0.2);
}

.profile-avatar img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.profile-info {
  flex: 1;
}

.profile-name {
  font-size: 1.75rem;
  font-weight: 700;
  color: var(--yw-text-primary);
  margin: 0;
  line-height: 1.2;
}

.profile-title {
  font-size: 1rem;
  color: var(--yw-accent-green);
  margin: 0.25rem 0 0;
  font-weight: 600;
}

.profile-content {
  color: var(--yw-text-secondary);
  line-height: 1.7;
  margin-bottom: 1.5rem;
}

.profile-items {
  display: flex;
  flex-direction: column;
  gap: 0.75rem;
}

.profile-item {
  display: flex;
  align-items: center;
  gap: 1rem;
  padding: 0.625rem 1rem;
  background: var(--yw-tag-bg);
  border-radius: 8px;
  transition: all 0.3s ease;
}

.profile-item:hover {
  background: var(--yw-border);
  transform: translateX(8px);
}

.item-icon {
  color: var(--yw-accent-green);
  font-size: 1.25rem;
  width: 1.5rem;
  text-align: center;
}

.item-text {
  color: var(--yw-text-primary);
  font-size: 1rem;
  flex: 1;
}

@keyframes slideUp {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>