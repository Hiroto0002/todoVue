<script setup>
import { ref } from "vue"
const newWord = ref('') 
const task = ref([
  
])
const message = ref('')
</script>

<template>
<form>
  <input v-modle="newWord">
  <button>I'DO</button>
</form>
<ul>
  <li >
    {{ message.text }}
  </li>
</ul>
</template>