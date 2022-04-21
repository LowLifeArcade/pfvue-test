<script setup>
import { ref, computed } from 'vue';

import HelloWorld from './components/HelloWorld.vue';
const number = ref(5);
const count = ref(12);
const stuff = computed(() => {
  return number.value * 2;
});
</script>

<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <h1>{{ stuff }}</h1>
  <HelloWorld :count="count" />
  <button @click="number++">+</button>
  <button @click="number--">-</button>
  <h1>{{ count }}</h1>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
