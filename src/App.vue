<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <lottie-animation data="@/assets/patch-loading.json" />
    <lottie-animation data="@/assets/scratch-loading.json" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import LottieAnimation from './components/LottieAnimation.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    LottieAnimation,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
