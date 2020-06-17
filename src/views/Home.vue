<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/imgs/logo.png">
    <HelloWorld msg="此页面由Vue Cli编译"/>
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
