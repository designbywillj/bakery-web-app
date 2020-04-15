<template>
  <div class="container">
    <div class="row">
      <div class="col">
        <h1 class="title">Shop</h1>
      </div>
    </div>

    <div class="row">
      <div class="col--6">
        <n-link to="/product">
          <Card title="Baked Bread" description="$6.00" />
        </n-link>
      </div>
      <div class="col--6">
        <n-link to="/product">
          <Card title="Trdelnik" description="$6.00" />
        </n-link>
      </div>
      <div class="col--6">
        <n-link to="/product">
          <Card title="Macaroon Cake" description="$6.00" />
        </n-link>
      </div>
      <div class="col--6">
        <n-link to="/product">
          <Card title="Berry Cake" description="$6.00" />
        </n-link>
      </div>
      <div class="col--6">
        <n-link to="/product">
          <Card title="Chocolate Donut" description="$6.00" />
        </n-link>
      </div>
      <div class="col--6">
        <n-link to="/product">
          <Card title="Berry Cake" description="$6.00" />
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

<style lang="scss"></style>
