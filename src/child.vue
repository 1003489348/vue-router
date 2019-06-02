<template>
  <div id="app">
    <div id="nav">
      <div id="nav2">我是子组件</div>
      <div id="nav1"><router-link to="/">Home</router-link></div>
      <div id="nav1"><router-link to="/about">About</router-link></div>
      <div id="nav1"><router-link to="/chat">Chat</router-link></div>
    </div>
    <my></my>
  </div>
</template>


<script>
export default {
     
}
</script>


<style>
</style>
