<template>
  <div class="home">
    <h1>Home</h1>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  components: {
    HelloWorld
  }
}
</script>
<style>
.home{
  background: rgb(116, 111, 111);
  height: 500px;
  width: 100%;
}
</style>

