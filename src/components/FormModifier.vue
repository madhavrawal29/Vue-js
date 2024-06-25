<script setup>
import { ref } from 'vue'

const data = ref('')
</script>

<template>
  <div>
    <h2>Form Modifiers</h2>
    <!-- <input type="text" placeholder="Wait for outfocus" v-model.lazy="data" /> <br /> -->
    <!-- Wait for outfocus -->
    <!-- <input type="text" placeholder="remove spaces" v-model.trim="data" /> -->
    <!-- remove spaces -->
    <!-- <h3>Your text:{{ data }}</h3> -->
    <!-- <input type="text" placeholder="Data Type" v-model.number="data" /> -->
    <input type="text" placeholder="Data Type" v-model.number.lazy="data" />
    <h3>Data type : {{ typeof data }}</h3>
  </div>
</template>
