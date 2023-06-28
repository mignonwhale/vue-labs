<script setup lang="ts">

// 런타임 기반 선언
const props = defineProps({
  id: { type: String, required: true }, // wrapper type
  content: String,
  etc: { type: String, required: false, default: '기본값' },
  checked: Boolean
});

</script>

<template>
  <h1>Props 런타임 기반 선언 - 원시타입 + 기본값 설정</h1>
  <input type="checkbox" :checked="props.checked">
  <input type="text" :value="props.id">
  <input type="text" :value="props.content">
  <input type="text" :value="props.etc">
</template>

<style scoped></style>