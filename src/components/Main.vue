<template>
  <section>

      <Performance />
      <Numbers />
      <Excellence />
      <Team />
      <News />
      <Lead />
      <Touch />
      
  </section>
</template>

<script>
import Performance from "./Performance.vue"
import Numbers from "./Numbers.vue"
import Excellence from "./Excellence.vue"
import Team from "./Team.vue"
import News from "./News.vue"
import Lead from "./Lead.vue"
import Touch from "./Touch.vue"

export default {
    name: "Main",
    components: {
      Performance,
      Numbers,
      Excellence,
      Team,
      News,
      Lead,
      Touch
    }
}
</script>

<style>

</style>