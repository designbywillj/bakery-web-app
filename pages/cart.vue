<template>
  <div class="container">
    <div class="row">
      <div class="col">
        <h1 class="title">Cart</h1>
      </div>
    </div>

    <div class="row">
      <div class="col--12">
        <CartItem title="Baked Bread" description="$6.00" />
      </div>
      <div class="col--12">
        <CartItem title="Baked Bread" description="$6.00" />
      </div>
      <div class="col--12">
        <CartItem title="Baked Bread" description="$6.00" />
      </div>
    </div>

    <div class="row">
      <div class="col--12">
        <div>Subtotal</div>
        <div class="cart__total">$18.00</div>
      </div>
    </div>

    <div class="row">
      <div class="col--12">
        <Button text="Continue Shopping" secondary />
      </div>
      <div class="col--12">
        <Button class="cart__submit" text="Check Out" primary />
      </div>
    </div>
  </div>
</template>

<script>
import Button from '@/components/Button'
import CartItem from '@/components/CartItem'

export default {
  components: {
    Button,
    CartItem
  }
}
</script>

<style lang="scss">
.cart {
  &__total {
    margin-top: 0.25rem;
    margin-bottom: 2rem;
    font-size: 1.5rem;
    font-weight: 700;
  }

  &__submit {
    margin-top: 1rem;
    margin-bottom: 3rem;
  }
}
</style>
