<script setup>
const props = defineProps({ name: String, user: Object, func1: Function })
</script>

<template>
  <div>
    <h3>Child Component</h3>
    <h2>Fetched Name from Parent component --> {{ name }}</h2>
    <h2>Fetched Object from Parent component --> {{ user.name }} and email {{ user.email }}</h2>
    <button @click="func1" type="button">Button to call Parent Function</button>
  </div>
</template>
