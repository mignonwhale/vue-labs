<script setup lang="ts">
interface Todo {
  id: string
  content: string
  etc?: string
  checked: boolean
}
const props = defineProps<{ todo: Todo }>()
</script>

<template>
  <h1>2-2. Props 타입기반 선언 - 제네릭 인자로 인터페이스 전달</h1>
  <input type="checkbox" :checked="props.todo.checked" />
  <input type="text" :value="props.todo.id" />
  <input type="text" :value="props.todo.content" />
  <input type="text" :value="props.todo.etc" />
</template>

<style scoped></style>
