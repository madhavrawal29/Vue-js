<template>
  <!-- <h1>My First Component {{ 10 + 10 }}</h1>
  <h1>My email {{ email }}</h1>
  <h1>My Name {{ name }}</h1>
  <h2>My Changed Name {{ (name = 'Maddy') }}</h2>
  <h2>Function inside function and my age {{ age() }}</h2>
  <h2>My height Function with Parameter {{ height('5,4') }}</h2> -->

  <!-- Methods -->
  <!-- <br /><br />
  <h2>My name throught Methods {getName()}</h2> -->

  <!-- Events Handling -->
  <!-- <button @click="clickfn()">Button</button>
  <br />
  <button @dblclick="doubleClickfn('Double clicked button')">Double Click Button</button>
  <br />
  <button @mousemove="doubleClickfn('Mouse Move button')">Mouse Move Button</button>
  <br />
  <h1>Count value {{ count }}</h1>
  <button @click="increaseCount">Click to increase count</button> -->
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
      },
      count: 0
    }
  },
  methods: {
    clickfn() {
      alert('Hey Im clicked')
    },
    doubleClickfn(message) {
      console.warn(message)
    },
    increaseCount() {
      this.count += 1
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
