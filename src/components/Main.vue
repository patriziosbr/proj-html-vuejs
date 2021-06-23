<template>
  <section>

      <Performance />
      <Numbers />
      <Excellence />
      <Team />
      
  </section>
</template>

<script>
import Performance from "./Performance.vue"
import Numbers from "./Numbers.vue"
import Excellence from "./Excellence.vue"
import Team from "./Team.vue"

export default {
    name: "Main",
    components: {
      Performance,
      Numbers,
      Excellence,
      Team
    }
}
</script>

<style>

</style>