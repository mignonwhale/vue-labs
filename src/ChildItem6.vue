<script setup lang="ts">
interface Todo {
  id: string
  content: string
  etc?: string
  checked: boolean
}

const props = withDefaults(defineProps<Todo>(), {
  id: '',
  content: '',
  etc: '기본값2',
  checked: false
})
</script>

<template>
  <h1>2-2-1. Props 타입기반 선언 - 인터페이스 기본값 설정</h1>
  <input type="checkbox" :checked="props.checked" />
  <input type="text" :value="props.id" />
  <input type="text" :value="props.content" />
  <input type="text" :value="props.etc" />
</template>

<style scoped></style>
