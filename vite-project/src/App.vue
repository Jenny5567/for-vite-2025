<script setup>
import { ref } from 'vue'; // 把ref從vue導入

  const num = ref(1);
  function clickMe() {
    num.value ++;
  }
  //不用return
      
</script>

<template>
  <div id="app">
    {{ num }}
    <button type="button" v-on:click="clickMe">點我</button> 
    <!-- v-on:click="clickMe" 事件綁定 -->
  </div>
</template>


