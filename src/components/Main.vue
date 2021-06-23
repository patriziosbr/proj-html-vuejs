<template>
  <section>

      <Performance />
      <Numbers />
      <Excellence />
      <Team />
      <News />
      
  </section>
</template>

<script>
import Performance from "./Performance.vue"
import Numbers from "./Numbers.vue"
import Excellence from "./Excellence.vue"
import Team from "./Team.vue"
import News from "./News.vue"

export default {
    name: "Main",
    components: {
      Performance,
      Numbers,
      Excellence,
      Team,
      News
    }
}
</script>

<style>

</style>