<template>
 <div>
     <button v-onclick="upFunction()" class="btn-btn-info">{{lable}}</button>
     <button @click="downFunction()" class="btn-btn-info ml-3">-</button>
     <p v-bind:style="{fontSize:fsize+'px'}"> {{Counter}} </p>
     
</div> 
</template>

<script>
export default {
    data: function(){
        return{
            counter: 0,    
            fsize: 50,
        }
    },

    props:{
        lable: String,
    },

    method:{
        upFunction: function(){
            this.counter +=1
            this.fsize +=10

            console.log(this.fsize);
            console.log(this.counter);
        },
        downFunction: function(){
            this.counter -=1
            this.fsize -=10

            console.log(this.fsize);
            console.log(this.counter);
        },
    },
}
</script>

<style>

</style>