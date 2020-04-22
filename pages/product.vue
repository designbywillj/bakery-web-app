<template>
  <div class="container">
    <div class="row">
      <div class="col">
        <h2 class="product__title">Baked Bread</h2>
        <div class="product__price">$6.00</div>
      </div>
    </div>

    <div class="row">
      <div class="col--12">
        <div class="product__img"></div>
      </div>
    </div>

    <div class="row">
      <div class="col--12">
        <Button class="product__add" text="Add To Cart" primary />
      </div>
    </div>

    <div class="row">
      <div class="col--12">
        <h3 class="product__heading">Description</h3>
        <p class="product__description">
          Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
          nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
          reprehenderit in voluptate velit esse cillum dolore eu fugiat aute
          irure nulla pariatur.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import Button from '@/components/Button'

export default {
  components: {
    Button
  }
}
</script>

<style lang="scss">
@import '@/assets/scss/_colors.scss';

.product {
  &__title {
    margin-top: 2rem;
    margin-bottom: 0.5rem;
    line-height: 3rem;
  }

  &__price {
    margin-bottom: 2rem;
  }

  &__img {
    width: 100%;
    height: 240px;
    margin-bottom: 3rem;
    border-radius: 1rem;
    background-color: $color--gray;
  }

  &__add {
    margin-bottom: 3rem;
  }

  &__heading {
    margin-bottom: 1rem;
  }

  &__description {
    margin-bottom: 3rem;
  }
}
</style>
