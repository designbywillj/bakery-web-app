<template>
  <div class="container">
    <div class="row">
      <div class="col">
        <h1 class="title">Explore</h1>
      </div>
    </div>

    <div class="row">
      <div class="col--12">
        <n-link to="/shop">
          <Card title="Bread" />
        </n-link>
      </div>
      <div class="col--12">
        <n-link to="/shop">
          <Card title="Cakes" />
        </n-link>
      </div>
      <div class="col--12">
        <n-link to="/shop">
          <Card title="Donuts" />
        </n-link>
      </div>
    </div>
  </div>
</template>

<script>
import Card from '@/components/Card'

export default {
  components: {
    Card
  }
}
</script>
