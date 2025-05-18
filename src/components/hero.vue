<template>
  <div class="hero">
    <div class="hero__title">
      <h1>Unleash the Beast:</h1>
      <h1 class="hero__title-2">Power Through the Mist</h1>
    </div>
    <div class="hero__subtitle">
      <p>
        The Lamborghini Huracán STO is a track-focused <br />
        supercar that combines the best of both worlds: a <br />high-performance
        sports car with the versatility <br />
        to be driven on the road.
      </p>
    </div>
    <div class="hero__button">
      <button>Book a Test Drive</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeroSection',
}
</script>

<style scoped lang="scss">
.hero {
  height: calc(100vh - 108px);
  width: 100%;
  display: flex;
  align-items: center;
  color: #fffff0;
  justify-content: center;
  flex-direction: column;

  &__title {
    font-size: 3rem;
    text-align: center;
    font-style: italic;

    &-2 {
      font-size: 4rem;
      margin-top: -1rem;
      text-align: center;
      font-style: normal;
      font-family: 'Inter', serif;
    }
  }

  &__subtitle {
    font-size: 1rem;
    text-align: center;
  }

  &__button {
    margin-top: 2rem;
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
