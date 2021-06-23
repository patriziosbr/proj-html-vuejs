<template>
  <section>

      <Performance />
      <Numbers />
      <Excellence />
      <Team />
      <News />
      <Lead />
      
  </section>
</template>

<script>
import Performance from "./Performance.vue"
import Numbers from "./Numbers.vue"
import Excellence from "./Excellence.vue"
import Team from "./Team.vue"
import News from "./News.vue"
import Lead from "./Lead.vue"

export default {
    name: "Main",
    components: {
      Performance,
      Numbers,
      Excellence,
      Team,
      News,
      Lead
    }
}
</script>

<style>

</style>