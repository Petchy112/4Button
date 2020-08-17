<template>
  <div>
    <button v-on:click="counter += 1">{{label}}
        <!--like+1
        dislike-10
        love+5
        reset-->
    </button>
    <h2>{{ counter }}</h2>
  </div>
</template>

<script>
export default {
  name: "CsButton",
  props: {
      label: String
  },
  data: function () {
    return {
      counter: 0,
      classObject: {
          active: true,
          'text-danger': false,
          weight: 20,
      }
    };
  },
};
</script>

<style>
</style>