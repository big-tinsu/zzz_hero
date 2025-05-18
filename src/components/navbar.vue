<template>
  <nav class="navbar">
    <div class="navbar__logo">
      <p>Drive<span>Through</span></p>
    </div>
    <div class="navbar__links">
      <ul>
        <li v-for="link in links" :key="link.id">{{ link.name }}</li>
      </ul>
    </div>
    <div class="navbar__button">
      <button>Watch Demo</button>
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
  color: #fffff0;
  justify-content: space-between;
  align-items: center;
  box-sizing: border-box;
  height: 108px;
  padding: 1rem 2rem;
  background-color: transparent;

  &__logo {
    p {
      font-size: 1.5rem;
      font-weight: 400;
      span {
        font-weight: 300;
        color: #888888;
      }
    }
  }

  &__links {
    display: flex;
    ul {
      display: flex;
      gap: 2rem;
      list-style: none;
      li {
        cursor: pointer;
        font-size: 1rem;
      }
    }
  }
  &__button {
    margin-top: 2rem;
    height: 100%;
    button {
      background: linear-gradient(to bottom, #000000, #1a1a1a);
      border: none;
      color: #fffff0;
      font-size: 1rem;
      padding: 1rem 2rem;
      border-radius: 1.2rem;
      cursor: pointer;
    }
  }
  @media (max-width: 1024px) {
    display: none;
  }
}
</style>
