<script setup>
import { computed, ref } from 'vue'

const isActive = ref(true)

const classObject = computed(() => ({
  title: isActive.value,
  err: true,
  other: true
}))
</script>

<template>
  <div>
    <h1 :class="classObject">Css Class Binding</h1>
    <button @click="isActive = !isActive">Apply Style</button>
  </div>
</template>

<style>
.title {
  background-color: skyblue;
}
.err {
  color: red;
  font-weight: bold;
}
.other {
  font-size: 50px;
}
</style>
