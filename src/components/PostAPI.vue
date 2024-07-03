<script setup>
import { ref } from 'vue'
import axios from 'axios'

const email = ref('')
const password = ref('')

const onSendData = async () => {
  //   console.log(email.value, password.value)
  let result = await axios.post('https://dummy.restapiexample.com/api/v1/create', {
    email: email.value,
    password: password.value
  })
  console.log('Result', result)
}
</script>
<template>
  <div>
    <h1>Post API</h1>
    <div class="form-data">
      <input v-model="email" type="text" placeholder="Enter email" /> <br />
      <input v-model="password" type="password" placeholder="Enter Password" /> <br />
      <button @click="onSendData">Send Data</button>
    </div>
  </div>
</template>
