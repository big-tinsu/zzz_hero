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

  <div class="hero__mobile">
    <p>This content is not available on mobile devices.</p>
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
  @media (max-width: 1024px) {
    display: none;
    /* max-height: calc(100vh - 108px);
    padding: 2rem 1rem; */
  }
  /* @media (max-width: 600px) {
    .hero__title {
      font-size: 1.2rem;
      &-2 {
        font-size: 1.5rem;
      }
    }
    .hero__subtitle {
      font-size: 0.85rem;
    }
    .hero__button button {
      font-size: 0.85rem;
      padding: 0.7rem 1rem;
    }
  } */
}

.hero__mobile {
  display: none;
  @media (max-width: 1024px) {
    display: block;
    background-color: #1a1a1a;
    width: 100%;
    height: 100%;
    p {
      font-size: 1.2rem;
      text-align: center;
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
