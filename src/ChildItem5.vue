<script setup lang="ts">
const props = withDefaults(defineProps<{
  id: string
  content: string
  etc?: string
  checked: boolean
}>(), {
  id: '',
  content: '',
  etc: '기본값1',
  checked: false
})
</script>

<template>
  <h1>2-1-1. Props 타입기반 선언 - 객체 리터럴 기본값 설정</h1>
  <input type="checkbox" :checked="props.checked" />
  <input type="text" :value="props.id" />
  <input type="text" :value="props.content" />
  <input type="text" :value="props.etc" />
</template>

<style scoped></style>
