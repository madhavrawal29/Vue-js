<template>
  <h1>My First Component {{ 10 + 10 }}</h1>
  <h1>My email {{ email }}</h1>
  <h1>My Name {{ name }}</h1>
  <h2>My Changed Name {{ (name = 'Maddy') }}</h2>
  <h2>Function inside function and my age {{ age() }}</h2>
  <h2>My height Function with Parameter {{ height('5,4') }}</h2>

  <!-- Methods -->
  <br /><br />
  <h2>My name throught Methods {getName()}</h2>
</template>

<script>
export default {
  data() {
    return {
      email: 'mad@gmail.com',
      name: 'Madhav Rawal',
      age: function () {
        return 24
      },
      height: function (height) {
        return height
      },
      methods: {
        getName(name) {
          return name
        },
        getData() {
          return {
            name: 'Mads',
            age: this.age,
            height: this.height
          }
        }
      }
    }
  }
}
</script>

<style scoped>
h1 {
  color: red;
}
h2 {
  color: rgb(14, 154, 209);
}
</style>
