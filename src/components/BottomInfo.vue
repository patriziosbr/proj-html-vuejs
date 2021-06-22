<template>
  <section class="container-fuid bottom-bg d-flex align-items-center"> 
      <div class=" container  d-flex justify-content-between ">
        <p class="mb-0">Ejoy the low price. We are tracking any intention of piracy</p>
        <p class="mb-0">0x24B8 2020 NEXGEN is Proudly Powered by <span>Coding</span> </p>
      </div>

  </section>
</template>

<script>
export default {
    name: "BottomInfo"
}
</script>

<style lang="scss" scoped>
@import "../style/vars.scss";

    .bottom-bg {
        height: 50px;
        background-color: $bottom-info-bg;
        color: #fff;
        font-size: 13px;
        span {
            color: $primary-color;
        }
    }

</style>