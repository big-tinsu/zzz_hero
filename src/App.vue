<template>
  <NavBar
    :links="[
      { id: 1, name: 'Home' },
      { id: 2, name: 'About' },
      { id: 3, name: 'Cases' },
      { id: 4, name: 'Contact' },
    ]"
  />
  <HeroSection />
</template>

<script>
import HeroSection from './components/hero.vue'
import NavBar from './components/navbar.vue'
export default {
  name: 'App',
  components: {
    NavBar,
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
  font-family: 'Inter', serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-image: url('@/assets/images/hurucan.png');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;

  @media (max-width: 1024px) {
    color: #ffffff;
  }
}

#app::after {
  content: '';
  position: absolute;
  inset: 0;
  background-image: url('@/assets/images/screen.png');
  opacity: 0.7;
  pointer-events: none;
  mix-blend-mode: soft-light;
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
  font-family: 'Inter', serif;
  font-weight: 300;
  line-height: 1.5;
}
</style>
