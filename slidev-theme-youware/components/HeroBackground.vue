<template>
  <div class="hero-background">
    <div class="gradient-orb orb-1"></div>
    <div class="gradient-orb orb-2"></div>
    <div class="gradient-orb orb-3"></div>
    <div class="pattern-overlay"></div>
    <div class="content-wrapper">
      <slot />
    </div>
  </div>
</template>

<style scoped>
.hero-background {
  position: relative;
  width: 100%;
  height: 100%;
  overflow: hidden;
}

.gradient-orb {
  position: absolute;
  border-radius: 50%;
  filter: blur(80px);
  opacity: 0.2;
  animation: float 20s infinite ease-in-out;
}

.orb-1 {
  width: 600px;
  height: 600px;
  background: radial-gradient(circle, var(--yw-accent-green) 0%, transparent 70%);
  top: -200px;
  left: -200px;
  animation-delay: 0s;
}

.orb-2 {
  width: 800px;
  height: 800px;
  background: radial-gradient(circle, #6B8E6B 0%, transparent 70%);
  bottom: -300px;
  right: -300px;
  animation-delay: 7s;
}

.orb-3 {
  width: 500px;
  height: 500px;
  background: radial-gradient(circle, var(--yw-tag-bg) 0%, transparent 70%);
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  animation-delay: 14s;
}

.pattern-overlay {
  position: absolute;
  inset: 0;
  background-image: 
    repeating-linear-gradient(
      45deg,
      transparent,
      transparent 35px,
      rgba(77, 103, 65, 0.02) 35px,
      rgba(77, 103, 65, 0.02) 70px
    );
  pointer-events: none;
}

.content-wrapper {
  position: relative;
  z-index: 10;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

@keyframes float {
  0%, 100% {
    transform: translate(0, 0) scale(1);
  }
  25% {
    transform: translate(100px, -50px) scale(1.1);
  }
  50% {
    transform: translate(-50px, 100px) scale(0.9);
  }
  75% {
    transform: translate(50px, 50px) scale(1.05);
  }
}
</style>