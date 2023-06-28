<script setup lang="ts">

interface Todo {
  id: string,
  content: string,
  etc?: string,
  checked: boolean
}

// 타입기반 선언, 제네릭타입 인자에 넘겨준다.
const props = withDefaults(defineProps<Todo>(), {
  id: '',
  content: '',
  etc: 'default value',
  checked: false
});;


</script>

<template>
  <h1>Props 타입기반 선언 - 기본값 설정</h1>
  <input type="checkbox" :checked="props.checked">
  <input type="text" :value="props.id">
  <input type="text" :value="props.content">
  <input type="text" :value="props.etc">
</template>

<style scoped></style>