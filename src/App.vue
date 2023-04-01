<script setup>
import { ref } from "vue"
const newTask = ref('')
const tasks = ref([
  {text: 'aaaaa'}
])

function addTask() {
  tasks.value.push({ text: newTask.value })
  newTask.value = ''
} 

</script>

<template>
<form @submit.prevent="addTask">
  <input v-model="newTask">
  <button>NewTask</button>
</form>
<ul>
  <li v-for="task in tasks">
    {{ task.text }}
    <button>OK</button>
  </li>
</ul>
</template>