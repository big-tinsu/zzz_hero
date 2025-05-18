<template>
  <nav class="navbar">
    <div class="navbar__logo">
      <img src="@/assets/logo.png" alt="logo" />
    </div>
    <div class="navbar__links">
      <ul>
        <li v-for="link in links" :key="link.id">{{ link.name }}</li>
      </ul>
    </div>
    <div class="navbar__social">
      <ul>
        <li v-for="social in socials" :key="social.id">{{ social.name }}</li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'NavBar',
  props: {
    title: {
      type: String,
      required: true,
    },
    links: {
      type: Array,
      required: true,
    },
  },
}
</script>

<style scoped lang="scss">
.navbar {
  display: flex;
  color: #000;
  justify-content: space-between;
  align-items: center;
  padding: 1rem 2rem;
  background-color: transparent;

  &__links {
    display: flex;
    ul {
      display: flex;
      gap: 1rem;
      list-style: none;
    }
  }
}
</style>
