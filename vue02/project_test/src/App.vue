<template>
<!-- <p v-bind:href="www.naver.com">네이버로 이동</p>
<a :href="www.naver.com">2</a>
<a v-on:click="dosomething">1</a> -->
<!-- <p v-on:click="dosomething">버튼</p> -->
<p v-on:keyup.a="dosomething">버튼</p>
<!-- <input v-on:keyup.a="KeyPrint"/> -->
<input :value="state.key" v-on:keyup.a="KeyPrint"/>
</template>
<script setup>

import { reactive } from 'vue';

let state = reactive({
key="";

})
function dosomething(){
  console.log("click")
} 

  // function dosomething(){
  //   console.log("클릭");
  // }

  // function KeyPrint(){
  //   console.log("");
  // }
</script>