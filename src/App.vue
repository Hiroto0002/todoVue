<script setup>
import { ref } from 'vue'
const message = ref('')

</script>

<template>
  <input v-model="message" placeholder="edit me" />
  <button>ボタン</button>
</template>
