<template>
  <div>
    <button v-on:click="counter += 1">{{like}}</button>
    <button v-on:click="counter += 10">{{love}}</button>
    <button v-on:click="counter -= 10">{{dislike}}</button>
    <button v-on:click="counter = 0">{{reset}}</button>
    <h2>{{counter}}</h2>
  </div>
</template>

<script>
export default {
  name: 'CsButton',
  props: {
      label:Image,
      
  },
  data: function () {
    return {
      counter: 0,
      }
    },
};
</script>

<style>
</style>