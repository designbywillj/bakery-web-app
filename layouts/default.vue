<template>
  <div id="app">
    <Header />

    <main>
      <nuxt />
    </main>
  </div>
</template>

<script>
import Header from '@/components/Header'

export default {
  components: {
    Header
  }
}
</script>

<style lang="scss">
.page-enter-active,
.page-leave-active {
  transition: opacity 0.25s ease-in-out;
}
.page-enter,
.page-leave-active {
  opacity: 0;
}
</style>
