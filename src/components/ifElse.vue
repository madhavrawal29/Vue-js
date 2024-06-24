<script setup>
import { ref } from 'vue'

const awesome = ref(true)
</script>
<template>
  <div>
    <button @click="awesome = !awesome">Toggle</button>
    <h1 v-if="awesome">Vue is awesome (If Condition)</h1>
    <h1 v-else>Oh no (else condition)</h1>
  </div>
</template>
