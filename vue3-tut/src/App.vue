<template>
  <!-- <componentA></componentA> -->
  <!-- <p>{{dataList[0]}}</p>
  <p>{{dataList[1]}}</p>
  <p>{{dataList[2]}}</p>
  <p>{{dataList[3]}}</p> -->
  <p v-for="text in dataList">{{text}}</p>
</template>

<script setup>
    // import componentA from './components/componentA.vue';
    const dataList = [
      'a','b','c','d'
    ]
</script>


<style scoped>
</style>
