<template>
  <div class="slidev-layout cover">
    <slot />
  </div>
</template>

<style>
/* Reset all scaling and positioning for cover slides */
.slidev-page:has(.slidev-layout.cover) {
  position: fixed !important;
  top: 0 !important;
  left: 0 !important;
  width: 100vw !important;
  height: 100vh !important;
  transform: none !important;
  z-index: 10000 !important;
}

.slidev-layout.cover {
  width: 100vw !important;
  height: 100vh !important;
  position: absolute !important;
  top: 0 !important;
  left: 0 !important;
  padding: 0 !important;
  margin: 0 !important;
  overflow: hidden !important;
}

.slidev-layout.cover .absolute {
  position: absolute !important;
  top: 0 !important;
  left: 0 !important;
  right: 0 !important;
  bottom: 0 !important;
}

.slidev-layout.cover img {
  width: 100vw !important;
  height: 100vh !important;
  object-fit: cover !important;
  object-position: center !important;
}

/* Override Slidev's slide container scaling for cover slides */
#slide-content:has(.slidev-layout.cover) {
  transform: none !important;
  width: 100vw !important;
  height: 100vh !important;
  position: fixed !important;
  top: 0 !important;
  left: 0 !important;
}
</style>
