<template>
  <!-- <componentA></componentA> -->
  <!-- <p>{{dataList[0]}}</p>
  <p>{{dataList[1]}}</p>
  <p>{{dataList[2]}}</p>
  <p>{{dataList[3]}}</p> -->
  <!-- <p v-for="text in dataList">{{text}}</p> -->
  <!-- <p v-for="(value,key,index) in dataList">
    <span v-show="key !== 'key3'">{{index}}{{key}}:{{value}}</span>
  </p> -->
  <!-- <p v-for="text in dataLists">{{text}}</p> -->

  <!-- <p class="test-cls" :key="test">{{ test }}</p> -->

  <h1>Computed 計算屬性</h1>
  <h3>{{num * 100}}%</h3>
  
</template>

<script setup>
// import componentA from './components/componentA.vue';
// import { ref } from 'vue'
// const test = ref("test");
// const dataList = [
//   'a', 'b', 'c', 'd', '123', 'abcd'
// ]
// const dataLists = {
//   key1: 'ab',
//   key2: 'bc',
//   key3: 'cd',
//   key4: 'de',
// }

// setTimeout(()=>{
//   test.value = 'apple!'
// },2000)


const num = 0.6;

</script>


<style scoped>
#app {
  font-family: Arial, Helvetica, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.test-cls {
  font-size: 40px;
  animation: openIn 1s ease-in-out;
}
@keyframes openIn{
  0%{
    opacity: 0;
    transform: translatey(20px);
  }
  100%{
    opacity: 1;
    transform: translatey(0);
  }
}
</style>
