<template>
  <div class="container">
    <div class="row">
      <div class="col">
        <h1 class="title">Contact</h1>
      </div>
    </div>

    <div class="row">
      <div class="col--12">
        <Input label="Name" text />
      </div>
      <div class="col--12">
        <Input label="Email" email />
      </div>
      <div class="col--12">
        <Input label="Message" textarea />
      </div>
      <div class="col--12">
        <Button text="Send" primary />
      </div>
    </div>
  </div>
</template>

<script>
import Input from '@/components/Input'
import Button from '@/components/Button'

export default {
  components: {
    Input,
    Button
  }
}
</script>

<style lang="scss">
.map {
  width: 100%;
  height: 240px;
  margin-top: 3rem;
  margin-bottom: 3rem;
  border-radius: 1rem;
}
</style>
