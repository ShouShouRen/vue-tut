<template>
    <button v-on:click="changeView(1)">顯示單向綁定</button>
    <button @click="changeView(2)">顯示雙向綁定</button>
    <button @click="changeView(3)">沒畫面</button>

    <div>
        <p>Hello World</p>
    </div>

    <!-- <div class="container-1" v-if="view === 1">
        <p>資料的單向綁定</p> -->
        <!-- 資料的單向綁定 -->
        <!-- {{ data }} -->
    <!-- </div> -->

    <!-- <div class="container-2" v-if="view === 2"> -->
        <!-- 資料的雙向綁定 -->
        <!-- <p>資料的雙向綁定</p> -->
        <!-- <input type="text" v-model="text">
        <p>{{ text }}</p>
    </div>

    <div v-if="view !== 1 && view !== 2">沒畫面</div> -->

    <!------------ v-show ------------>
    <div class="container-1" v-show="view === 1">
        <p>資料的單向綁定</p>
        {{ data }}
    </div>

    <div class="container-2" v-show="view === 2">
        <p>資料的雙向綁定</p>
        <input type="text" v-model="text">
        <p>{{ text }}</p>
    </div>

    <div v-show="view !== 1 && view !== 2">沒畫面</div>
</template>

<script setup>
import { ref } from "@vue/reactivity";

const data = "Hello Vue";
// ref可使資料同步
const text = ref("123");

const view = ref(1);

const changeView = (index) => {
    view.value = index;
}
// const changeView2 = () => {
//     view.value = 2;
// }


</script>


<style scoped>
.container-1 {
    border: 2px solid #f00;
}

.container-2 {
    border: 2px solid skyblue;
}
</style>
