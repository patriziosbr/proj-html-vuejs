<template>
    <section>

        <TopInfo />

        <Jumbotron :navTags="navArr" />


    </section>
</template>

<script>
import TopInfo from "./TopInfo.vue"
import Jumbotron from "./Jumbotron.vue"


export default {
    name: "Header",
    props: [ "navArr" ],
    components: {
        TopInfo,
        Jumbotron
    }
}
</script>

<style lang="scss" scoped>


</style>