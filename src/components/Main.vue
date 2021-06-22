<template>
  <section>

      <Performance />
      <Numbers />
      
  </section>
</template>

<script>
import Performance from "./Performance.vue"
import Numbers from "./Numbers.vue"

export default {
    name: "Main",
    components: {
      Performance,
      Numbers
    }
}
</script>

<style>

</style>