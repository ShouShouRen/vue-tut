<template>
    <p>Hello World</p>

    <p>資料的單向綁定</p>
    <!-- 資料的單向綁定 -->
    {{ data }}

    <!-- 資料的雙向綁定 -->
    <p>資料的雙向綁定</p>
    <input type="text" v-model="text">
    <p>{{text}}</p>
</template>

<script setup>
import { ref } from "@vue/reactivity";

const data = "Hello Vue";
// ref可使資料同步
const text = ref("123");
</script>


<style scoped>
</style>
