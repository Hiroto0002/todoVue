<script setup>
import { ref } from "vue"
const x = ref(true)
function y() {
  x.value = !x.value
}
</script>

<template>
<div>
  <button @click="y">文字が変わるよ</button>
  <h1 v-if="x">もとの文字</h1>
  <h1 v-else>かわった文字</h1>
</div>
</template>