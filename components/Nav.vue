<template>
  <nav class="nav">
    <div class="nav__container">
      <n-link to="/" class="nav__link">Explore</n-link>
      <n-link to="/shop" class="nav__link">Shop</n-link>
      <n-link to="/about" class="nav__link">About</n-link>
      <n-link to="/contact" class="nav__link">Contact</n-link>
    </div>
  </nav>
</template>

<script>
export default {}
</script>

<style lang="scss">
@import '@/assets/scss/_colors.scss';

.nav {
  position: fixed;
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  background-color: #59364080;
  z-index: 1;
  transition: opacity 0.25s cubic-bezier(0, 0, 0.5, 1);

  &__container {
    width: 80%;
    height: 100%;
    padding: 2rem 1.5rem;
    background-color: $color--white;
    transition: transform 0.25s cubic-bezier(0, 0, 0.5, 1);
  }

  &__link {
    margin-bottom: 1rem;
    display: block;
    font-size: 2.25rem;
    line-height: 3rem;

    &.nuxt-link-exact-active {
      font-weight: 700;
    }
  }

  &.hidden {
    opacity: 0;
    pointer-events: none;

    .nav__container {
      transform: translateX(-100vw);
    }
  }
}
</style>
