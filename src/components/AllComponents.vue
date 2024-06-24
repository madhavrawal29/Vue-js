<!-- AllComponents.vue -->
<script setup>
import GettingInputValue from './GettingInputValue.vue'
import ifElse from './ifElse.vue'
</script>

<template>
  <div class="container">
    <h1>ALL COMPONENTS</h1>
    <!-- <GettingInputValue /> -->
    <ifElse />
  </div>
</template>

<style scoped>
.container {
  position: absolute;
  top: 10px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  h1 {
    font-size: 40px;
    margin-bottom: 10px;
    font-weight: bold;
    text-decoration: underline;
  }
}
</style>
