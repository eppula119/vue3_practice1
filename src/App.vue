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
    <template v-slot:title><h1>ユーザ情報</h1></template>
    
    <template v-slot:default>
      <div>
        <div>John Doe</div>
        <div>Jane Doe</div>
      </div>
    </template>
    <template v-slot:actions><button>ユーザ追加</button></template>
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