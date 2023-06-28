<script setup lang="ts">
import ChildItem1 from './ChildItem1.vue';
import ChildItem2 from './ChildItem2.vue';

const todo = { id: '1', content: 'test1', checked: true }
</script>

<template>
  <ChildItem1 :id="todo.id" :content="todo.content" :checked="todo.checked"></ChildItem1>
  <ChildItem2 :todo="todo"></ChildItem2>
</template>

<style scoped></style>
