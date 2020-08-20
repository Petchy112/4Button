<template>
  <div id="app">
    <h1>LOOK AT YOU NOW LOOK AT ME !</h1>
    <div class="row">
      <div class="col-6">
        <img alt="" src="./assets/pic4.jpg" width="500px" >
      </div>
      <div class="col-6">
        <img alt="" src="./assets/pro.jpg" width="500px" >
      </div>  
    </div> 
  
    <div class="row">
      <div class="col-6"><CsButton/></div>
      <div class="col-6"><CsButton/></div>
      
    </div>
  </div>
</template>

<script>
import CsButton from './components/CsButton.vue'

export default {
  name: 'App',
  components: {
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
  margin: 60px;
  padding: 60px;
}

</style>
