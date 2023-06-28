<script setup lang="ts">

interface Todo {
  id: string,
  content: string,
  checked: boolean
}

// 타입기반 선언, 제네릭타입 인자에 넘겨준다.
const props = defineProps<{
  todo: Todo
}>();

</script>

<template>
  <h1>객체 props</h1>
  <input type="checkbox" :checked="props.todo.checked">
  <input type="text" :value="props.todo.id">
  <input type="text" :value="props.todo.content">
</template>

<style scoped></style>