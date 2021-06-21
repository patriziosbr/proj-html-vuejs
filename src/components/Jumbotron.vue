<template>
  <section>
        <div class="jumbotron container-fluid">
            <nav class="container">
                <div>
                    <a href="/">
                        <p>logo</p>
                    </a>
                </div>
            </nav>
            <div>

            </div>
        </div>
  </section>
</template>

<script>
export default {
    name: "Jumbotron"

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