<template>
  <HelloWorld msg="Welcome to Your Vue.js App" />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
  },
}
</script>

<style>
#app {
  font-family: 'Inter', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: 'Instrument Serif', serif;
  font-weight: 400;
}

body {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  line-height: 1.5;
}
</style>
