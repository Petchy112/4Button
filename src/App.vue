<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    <div class="row">
      <div class="col-6"><CsButton label="like"/></div>
      
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import CsButton from './components/CsButton.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    CsButton,
  },
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
