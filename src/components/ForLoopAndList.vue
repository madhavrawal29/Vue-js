<script setup>
const technology = ['java', 'php', 'node', 'html']
const users = [
  {
    name: 'Madhav',
    email: 'madhav@gmail.com'
  },
  {
    name: 'Yashu',
    email: 'yashu@gmail.com'
  },
  {
    name: 'Rawal',
    email: 'rawal@gmail.com'
  }
]
</script>

<template>
  <div>
    <h1>Foor Loop through Array</h1>
    <ul>
      <li v-for="item in technology" :key="item">
        {{ item }}
      </li>
    </ul>
    <br />
    <br />
    <h1>Foor Loop through Objects</h1>
    <ul>
      <li v-for="data in users" :key="data.email">
        Name : {{ data.name }} <br />
        Email : {{ data.email }}
      </li>
    </ul>
  </div>
</template>
