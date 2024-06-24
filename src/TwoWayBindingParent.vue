<script setup>
import TwoWayBindingChild from './components/TwoWayBindingChild.vue'
import { ref } from 'vue'

// Define reactive properties
const msg = ref('Hello World!')
let count = ref(0)

// Define methods
const increaseCount = () => {
  count.value += 1
}
</script>

<template>
  <!-- Two way binding (V-Model) -->
  <h1>Two way Binding-->></h1>
  <input type="text" v-model="count" />
  <h2>Count value {{ count }}</h2>
  <button @click="increaseCount">Click to increase count</button>
  <br /><br />
  <br />
  <h1>{{ msg }}</h1>
  <TwoWayBindingChild v-model="msg" />
</template>
