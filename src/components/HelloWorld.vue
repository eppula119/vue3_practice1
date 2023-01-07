<script setup>
const props = defineProps({
  name: String,
});

const changeName = () => {
  props.name = 'Ken';
};
</script>

<template>
  <h2>子コンポーネント</h2>
  <p>Hello {{ props.name }}</p>
  <button @click="changeName">Change sName</button>
</template>