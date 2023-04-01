<script setup>
import { ref } from "vue"
const newTask = ref('')
const tasks = ref([
  {text: 'aaaaa'}
])

function removeTask(task) {
  tasks.value = tasks.value.filter((t) => )
}

</script>

<template>
<form @submit="addTask">
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