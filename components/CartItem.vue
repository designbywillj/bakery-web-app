<template>
  <div class="cart-item">
    <div class="cart-item__content">
      <div class="cart-item__img"></div>
      <div class="cart-item__info">
        <div class="cart-item__title">{{ title }}</div>
        <div v-if="description" class="cart-item__description">
          {{ description }}
        </div>
      </div>
    </div>
    <button type="button" class="cart-item__button">
      <img src="/icons/icon-close.svg" alt="Remove" />
    </button>
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

.cart-item {
  margin-bottom: 2rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  text-decoration: none;

  &__content {
    display: flex;
    align-items: center;
  }

  &__img {
    flex: 0 0 96px;
    width: 96px;
    height: 96px;
    background-color: $color--gray;
    border-radius: 1rem;
  }

  &__info {
    margin-left: 1.5rem;
  }

  &__title {
    font-size: 1.5rem;
    font-weight: 700;
    line-height: 1.5rem;
  }

  &__description {
    margin-top: 0.5rem;
    line-height: 1.5rem;
    justify-self: flex-start;
  }

  &__button {
    width: 24px;
    height: 24px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: transparent;
  }
}
</style>
