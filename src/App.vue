<script setup>
import Hello from './components/HelloWorld.vue';
import { ref } from 'vue';

const name = ref('John');
const changeName = () => {
  name.value = 'ssss'
}
</script>

<template>
  <h1>Vue 3 入門</h1>
  <Hello :name="name" />
  <button @click="changeName">Change Name</button>
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