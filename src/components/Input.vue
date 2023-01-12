<script setup>
const props = defineProps({
  modelVfalue: String,
});
</script>
<template>
  <input
    :value="props.modelVfalue"
    @input="$emit('update:modelVfalue', $event.target.value)"
    style="padding: 1em; border-radius: 1em; margin: 0.5em"
  />
</template>