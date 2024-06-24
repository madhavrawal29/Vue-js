<script>
export default {
  data() {
    return {
      email: null,
      password: null
    }
  },
  methods: {
    getData() {
      console.log('Get data: ', this.email, this.password)
    }
  }
}
</script>

<template>
  <div>
    <h1>GettingInputValue</h1>
    <input type="text" placeholder="enter email" v-model="email" /> <br /><br />
    <input type="password" placeholder="enter password" v-model="password" /> <br />
    <button @click="getData">Get Values</button>
  </div>
</template>
