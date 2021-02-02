<template>
  <div class="home">
    <img class="jpp" src="../assets/jpp.jpg">
    <HelloWorld msg="Give me a car"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

<style scoped>

.jpp {
  width:25%;
}

</style>
