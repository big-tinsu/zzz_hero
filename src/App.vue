<template>
  <HeroSection />
</template>

<script>
import HeroSection from './components/hero.vue'

export default {
  name: 'App',
  components: {
    HeroSection,
  },
}
</script>

<style>
html,
body {
  margin: 0;
  padding: 0;
}

#app {
  font-family: 'Inter', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: 'Instrument Serif', serif;
  font-weight: 400;
  margin: 0;
}

body {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  line-height: 1.5;
}
</style>
