<script setup>
import { ref } from 'vue';
import Input from './components/Input.vue';
import Hellow from './components/HelloWorld.vue';
import User from './components/User.vue';

const name = ref('John Doe');
const address = ref('');
</script>

<template>
  <h1>Vue 3 入門</h1>
  <User>
    <template v-slot:header="slotProps">
      <div>{{ slotProps }}</div>
    </template>
    <template v-slot:default="slotProps">
      <div>{{ slotProps }}</div>
    </template>
  </User>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>