<template>
  <section>
        <div class="jumbotron container-fluid">
            
            <NavBar :links="navTags"/>

            <Absolute />
          
        </div>
  </section>
</template>

<script>
import NavBar from "./NavBar.vue"
import Absolute from "./Absolute.vue"

export default {
    name: "Jumbotron",
    props: [ "navTags" ],
    components: {
        NavBar,
        Absolute
    }

}
</script>

<style lang="scss" scoped>
@import "../style/vars.scss";

    .jumbotron {
        height: 100vh;
        background-image: url(../assets/images/bg-2.jpg);
        background-size: cover;
        background-position: top;
    }

</style>