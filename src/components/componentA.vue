<template>
  <p>資料綁定 （單向綁定）</p>
  {{ data }}
  <p>資料綁定 （雙向綁定）</p>
  <input type="text" v-model="text">
  <p>{{text}}</p>
</template>

<script setup>
import { ref } from "@vue/reactivity";

const data = "Hello Vue Learning";
const text = ref("123");
</script>


<style>
</style>
