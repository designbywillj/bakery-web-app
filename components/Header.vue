<template>
  <header class="header">
    <button type="button" class="header__button" @click="toggle()">
      <img src="/icons/icon-menu.svg" alt="Menu" />
    </button>

    <Nav :class="{ hidden: !isMenuOpen }" @click.native="toggle()" />

    <nuxt-link to="/cart" class="header__button">
      <button type="button" class="header__button">
        <img src="/icons/icon-cart.svg" alt="Cart" />
      </button>
    </nuxt-link>
  </header>
</template>

<script>
import Nav from '@/components/Nav'

export default {
  components: {
    Nav
  },

  data: () => ({
    isMenuOpen: false
  }),

  methods: {
    toggle() {
      this.isMenuOpen = !this.isMenuOpen
    }
  }
}
</script>

<style lang="scss">
.header {
  padding: 0.75rem 0.75rem 0 0.75rem;
  display: flex;
  justify-content: space-between;

  &__button {
    width: 3rem;
    height: 3rem;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: transparent;
  }
}
</style>
