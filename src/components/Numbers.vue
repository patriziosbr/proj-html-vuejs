<template>
  <section class="container-fluid bg-car">
      <div class="container">

      </div>
  </section>
</template>

<script>
export default {
    name: "Numbers"
}
</script>

<style lang="scss" scoped>
    .bg-car {
        height: 600px;
        background-image: url(../assets/images/cars.jpg);
        background-position: center;
        background-size: cover;
        filter:  contrast(150%) grayscale(100%);
    }

</style>