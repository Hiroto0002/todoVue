<script setup>
import { ref } from "vue"
const newTask = ref('')
const tasks = ref([
  {text: 'aaaaa'}
])

function addTask() {
  tasks.value.push({ text: newTask.value })

} 

</script>

<template>
<form @submit.prevent="addTask">
  <input v-modle="newTask">
  <button>I'DO</button>
</form>
<ul>
  <li v-for="task in tasks">
    {{ task.text }}
    <button>NO</button>
  </li>
</ul>
</template>