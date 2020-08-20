<template>
        
    
  <div>
    <button v-on:click="counter += 1" class="button" id="blue"><i class="far fa-thumbs-up fa-2x"></i></button>
    <button v-on:click="counter += 10" class="button" id="red"><i class="far fa-heart fa-2x"></i></button>
    <button v-on:click="counter -= 10" class="button" id="gray"><i class="far fa-thumbs-down fa-2x"></i></button>
    <button v-on:click="counter = 0" class="button" id="black"><i class="fas fa-sync-alt fa-2x"></i></button>
    <h2>{{counter}}</h2>
  </div>
</template>

<script>
export default {
  name: 'CsButton',
  props: {
      label:String,
  },
  data: function () {
    return {
        counter: 0,
      }
    },
};
</script>

<style>
i{
  size: 9px;
}
.button {
  border:0 ;
  background-color:rgba(red, green, blue,0);
  padding: 47px;
  padding-top:20px ;
  padding-bottom: 20px;
  marker: pointer;
}
.button:hover{
  background-color: #ccc;
  
}
.button:active{
  background-color: black;
  #black{}
}
#blue {
  color: blue;
}


#red {
  color:red;
}
#gray{
  color: gray;
}
#black{
  color: black;
}
</style>