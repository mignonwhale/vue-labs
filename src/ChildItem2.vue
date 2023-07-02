<script setup lang="ts">
import type { PropType } from 'vue';

interface Todo {
  id: string
  content: string
  etc?: string // 선택입력값 표시 ?
  checked: boolean
}
const props = defineProps({ todo: Object as PropType<Todo> }) // 런타임기반에서 객체를 props로 받으려면 PropType을 이용한다. 
</script>

<template>
  <h1>1-2. Props 런타임기반 선언 - 객체 통으로 받기</h1>
  <input type="checkbox" :checked="props.todo?.checked" />
  <input type="text" :value="props.todo?.id" />
  <input type="text" :value="props.todo?.content" />
  <input type="text" :value="props.todo?.etc" />
</template>

<style scoped></style>
