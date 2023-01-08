<script setup>
  const props = defineProps({
    name: String
  })
  const emit  = defineEmits()
  const changeName = () => {
    emit('changeNameEvent')
  }
</script>

<template>
  <h2>子コンポーネント</h2>
  <p>Hello {{ props.name }}</p>
  <button @click="changeName">Change Name</button>
</template>