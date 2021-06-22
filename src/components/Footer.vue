<template>
<div>
  <section class="container-fluid">
      <BottomCards :dataOne="footOne"/>
  </section>
  <BottomInfo />

</div>
</template>

<script>
// import { component } from 'vue/types/umd'
import BottomCards from "./BottomCards.vue"
import BottomInfo from "./BottomInfo.vue"

export default {
    name: "Footer",
    props: ["footOne"],
    components: {
      BottomCards,
      BottomInfo
    }
}
</script>

<style lang="scss" scoped>
section.container-fluid {
  height: 450px;
  background-image: url(../assets/images/bg-7.jpg);
  background-position: center;
  background-size: cover;
}

</style>