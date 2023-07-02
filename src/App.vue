<script setup lang="ts">
import ChildItem1 from './ChildItem1.vue'
import ChildItem2 from './ChildItem2.vue'
import ChildItem3 from './ChildItem3.vue'
import ChildItem4 from './ChildItem4.vue'
import ChildItem5 from './ChildItem5.vue'
import ChildItem6 from './ChildItem6.vue'
import ChildItem7 from './ChildItem7.vue'


const todo = { id: '1', content: 'props로 전달한 내용', checked: true }
</script>

<template>
  <ChildItem1 :id="todo.id" :content="todo.content" :checked="todo.checked"></ChildItem1>
  <ChildItem2 :todo="todo"></ChildItem2>
  <ChildItem3 :id="todo.id" :content="todo.content" :checked="todo.checked"></ChildItem3>
  <ChildItem4 :todo="todo"></ChildItem4>
  <ChildItem5 :id="todo.id" :content="todo.content" :checked="todo.checked"></ChildItem5>
  <ChildItem6 :id="todo.id" :content="todo.content" :checked="todo.checked"></ChildItem6>
  <ChildItem7 :todo="todo"></ChildItem7>
</template>

<style scoped></style>
