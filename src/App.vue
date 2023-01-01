<script setup>
  let message = 'Hello Worl'

  const upperCase = () => {
    message = message.toUpperCase()
  }

  upperCase()
</script>

<template>
  <h1>Vue 3 入門練習</h1>
  <p v-text="message"></p>
</template>