<script setup>
import Child from './Child.vue'

const user = {
  name: 'Madhav',
  email: 'madhav@gmail.com'
}

const func1 = () => {
  alert('Parent Function Called')
}
</script>

<template>
  <div>
    <h1>Passing Data Parent To Child</h1>
    <h2>Parent Component</h2>
    <hr />
    <br />
    <br />
    <Child name="Madhav Rawal" :user="user" :func1="func1" />
  </div>
</template>
