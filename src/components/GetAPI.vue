<script setup>
import { ref, onMounted } from 'vue'
import axios from 'axios'

const list = ref([])

onMounted(async () => {
  let result = await axios.get('https://reqres.in/api/users?page=1')
  console.log(result.data.data)
  list.value = result.data.data
})
</script>

<template>
  <div>
    <h1>Get API</h1>
    <ul class="list-items" v-for="item in list" :key="item.id">
      <li>
        {{ item.id }}
      </li>
      <li>
        {{ item.first_name }}
      </li>
      <li>
        {{ item.email }}
      </li>
      <li>
        <img :src="item.avatar" :alt="item.first_name" />
      </li>
    </ul>
  </div>
</template>

<style scoped>
h1 {
  font-size: 40px;
  text-align: center;
}
.list-items {
  display: flex;
  li {
    list-style: none;
    border: 1px solid;
    width: 200px;
    height: 60px;
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: medium;
    background: cadetblue;
    color: black;
    font-family: cursive;
    border-radius: 15px;
  }
  img {
    width: 50px;
    height: 50px;
    border-radius: 50%;
  }
}
</style>
