<template>
    <section>

        <TopInfo />

        <Jumbotron />


    </section>
</template>

<script>
import TopInfo from "./TopInfo.vue"
import Jumbotron from "./Jumbotron.vue"


export default {
    name: "Header",
    components: {
        TopInfo,
        Jumbotron
    }
}
</script>

<style lang="scss" scoped>


</style>