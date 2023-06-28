<script setup lang="ts">

// 런타임 기반 선언
const props = defineProps({
  id: { type: String, required: true }, // wrapper type
  content: String,
  checked: Boolean
});

</script>

<template>
  <h1>원시타입 props</h1>
  <input type="checkbox" :checked="props.checked">
  <input type="text" :value="props.id">
  <input type="text" :value="props.content">
</template>

<style scoped></style>