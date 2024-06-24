<script setup>
import MyFirstComponent from './components/MyFirstComponent.vue'
import TwoWayBindingParent from './TwoWayBindingParent.vue'
import AllComponents from './components/AllComponents.vue'
import GettingInputValue from './components/GettingInputValue.vue'
</script>

<template>
  <header>
    <!-- <MyFirstComponent /> -->
    <!-- <TwoWayBindingParent /> -->
    <AllComponents />
  </header>
</template>

<style scoped>
header {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
