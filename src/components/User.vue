<script setup>
  const props = defineProps(['name']);
</script>

<template>
  <slot name="header" message="ヘッダー"></slot>
  <slot message="ユーザ" content="コンテント"></slot>
</template>