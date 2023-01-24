<script setup>
import { ref } from 'vue';
import Input from './components/Input.vue';
import Hellow from './components/HelloWorld.vue';
import User from './components/User.vue';
import Tokyo from './components/Tokyo.vue';
import Kyoto from './components/Kyoto.vue';

const name = ref('John Doe');
const address = ref('');
</script>

<template>
  <h1>Vue 3 入門</h1>
  <ul>
    <User>
      <template v-slot="{ user }">
        <li>{{ user.id }}</li>
      </template>
    </User>
    <Tokyo />
    <Kyoto />
  </ul>
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