<script setup lang="ts">
const props = defineProps<{
  id: string
  content: string
  etc?: string
  checked: boolean
}>()
</script>

<template>
  <h1>2-1. Props 타입기반 선언 - 제네릭 인자로 객체리터럴 전달</h1>
  <input type="checkbox" :checked="props.checked" />
  <input type="text" :value="props.id" />
  <input type="text" :value="props.content" />
  <input type="text" :value="props.etc" />
</template>

<style scoped></style>
