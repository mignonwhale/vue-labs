<script setup lang="ts">
interface Todo {
  id: string
  content: string
  etc?: string
  checked: boolean
}


const props = withDefaults(defineProps<{ todo: Todo }>(), {
  id: '',
  content: '',
  etc: '기본값2',
  checked: false
})
</script>

<template>
  <h1>test. Props 타입기반 선언 - 인터페이스 기본값 설정- 객체 통으로 넘기기</h1>
  <input type="checkbox" :checked="props.todo.checked" />
  <input type="text" :value="props.todo.id" />
  <input type="text" :value="props.todo.content" />
  <input type="text" :value="props.todo.etc" />
</template>

<style scoped></style>
