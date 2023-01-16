<script setup>
  const props = defineProps(['name']);
</script>

<template>
  <div>
    <slot name="title">ユーザー</slot>
  </div>
  <div>
    <slot>コンテンツ</slot>
  </div>
  <div>
    <slot name="actions">アクション</slot>
  </div>
</template>