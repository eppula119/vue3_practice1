<script setup>
import {ref} from 'vue'
const message = ref('Hello World');

const clickButton = () => {
  console.log(message.value);
};
</script>

<template>
  <h1>Vue 3 入門</h1>
  <p>{{ message }}</p>
  <input :value="message" @input="message = $event.target.value" />
  <div><button @click="clickButton">Click</button></div>
</template>

<style>
  .active {
    color: red;
    font-weight: 900
  }
  .underLine {
    text-decoration: underline;
  }
  .back {
    background-color: black;
  }
</style>