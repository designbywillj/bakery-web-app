<template>
  <div class="container">
    <div class="row">
      <div class="col">
        <h1 class="title">About</h1>
      </div>
    </div>

    <div class="row">
      <div class="col--12">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad
          minim veniam, quis nostrud exercitation ullamco laboris nisi ut
          aliquip ex ea commodo consequat.
        </p>
        <p>
          Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris
          nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
          reprehenderit in voluptate velit esse cillum dolore eu fugiat aute
          irure nulla pariatur.
        </p>
        <p>
          Excepteur sint occaecat cupidatat non proident, sunt in culpa qui
          officia deserunt mollit anim id est laborum officia deserunt.
        </p>
      </div>
    </div>

    <div class="row">
      <div class="col--12">
        <iframe
          class="map"
          width="100%"
          height="240"
          frameborder="0"
          style="border:0"
          src="https://www.google.com/maps/embed/v1/view?zoom=10&center=36.1627%2C-86.7816&key=AIzaSyD4iHGzKQRnVgkyXvNz6PIRMxpJRPCeDPM"
          allowfullscreen
        ></iframe>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
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
