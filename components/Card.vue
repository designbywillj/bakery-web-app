<template>
  <div class="card">
    <div class="card__img"></div>
    <div class="card__title">{{ title }}</div>
    <div v-if="description" class="card__description">{{ description }}</div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: ''
    },
    description: {
      type: String,
      default: ''
    }
  }
}
</script>

<style lang="scss">
@import '@/assets/scss/_colors.scss';
.card {
  margin-bottom: 3rem;
  text-decoration: none;

  &__img {
    width: 100%;
    height: 180px;
    background-color: $color--gray;
    border-radius: 1rem;
  }

  &__title {
    margin-top: 1rem;
    font-size: 1.5rem;
    font-weight: 700;
    line-height: 1.5rem;
  }

  &__description {
    margin-top: 0.5rem;
    line-height: 1.5rem;
  }
}
</style>
