<template>
  <!-- <componentA></componentA> -->
  <!-- <p>{{dataList[0]}}</p>
  <p>{{dataList[1]}}</p>
  <p>{{dataList[2]}}</p>
  <p>{{dataList[3]}}</p> -->
  <!-- <p v-for="text in dataList">{{text}}</p> -->
  <p v-for="(value,key,index) in dataList">
    <span v-show="key !== 'key3'">{{index}}{{key}}:{{value}}</span>
  </p>
  <!-- <p v-for="text in dataLists">{{text}}</p> -->
</template>

<script setup>
    // import componentA from './components/componentA.vue';
    const dataList = [
      'a','b','c','d','123','abcd'
    ]
    const dataLists = {
      key1:'ab',
      key2:'bc',
      key3:'cd',
      key4:'de',
    }
</script>


<style scoped>
</style>
