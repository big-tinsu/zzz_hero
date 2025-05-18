<template>
  <div class="hero">
    <h1>Hero</h1>
  </div>
</template>

<script>
export default {
  name: 'HeroSection',
}
</script>

<style scoped lang="scss">
.hero {
  background-image: url('@/assets/images/lambo.png');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  height: 100vh;
  width: 100%;
}

.hero::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url('@/assets/images/screen.png');
  opacity: 0.2;
  pointer-events: none;
  mix-blend-mode: soft-light;
}
</style>
