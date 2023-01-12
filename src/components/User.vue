<script setup>
  const props = defineProps(['name']);
</script>

<template>
  <p>このユーザーの名前は{{ props.name }}です。</p>
</template>