<script setup lang="ts">
import ChildItem1 from './ChildItem1.vue';
import ChildItem2 from './ChildItem2.vue';
import ChildItem3 from './ChildItem3.vue';
import ChildItem4 from './ChildItem4.vue';


const todo = { id: '1', content: 'test1', etc: '기타', checked: true }

</script>

<template>
  <ChildItem1 :id="todo.id" :content="todo.content" :checked="todo.checked"></ChildItem1>
  <ChildItem2 :id="todo.id" :content="todo.content" :checked="todo.checked"></ChildItem2>
  <ChildItem3 :todo="todo"></ChildItem3>
  <ChildItem4 :id="todo.id" :content="todo.content" :checked="todo.checked"></ChildItem4>
</template>

<style scoped></style>



