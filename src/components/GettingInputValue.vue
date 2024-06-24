<script>
export default {
  data() {
    return {
      email: null,
      password: null,
      technology: [],
      gender: []
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

    <!-- GET CHECKBOX AND RADIO BUTTON VALUE -->
    <h1>Get Checkbox and Radio Button Value</h1>
    <h3>Technology</h3>

    <label for="java">Java</label>
    <input type="checkbox" value="java" id="java" v-model="technology" />
    <br />
    <label for="php">Php</label>
    <input type="checkbox" value="php" id="php" v-model="technology" />
    <br />
    <label for="node">Node</label>
    <input type="checkbox" value="node" id="node" v-model="technology" />

    <h2>Selected Texhnologies --> {{ technology }}</h2>
    <br /><br />

    <h2>Gender</h2>
    <label for="male">Male</label>
    <input type="radio" name="gender" v-model="gender" value="male" id="male" />
    <br />
    <label for="female">Female</label>
    <input type="radio" name="gender" v-model="gender" value="female" id="female" />
    <br />
    <label for="other">Other</label>
    <input type="radio" name="gender" v-model="gender" value="other" id="other" />
    <br />
    <h2>Selected Gender --> {{ gender }}</h2>
  </div>
</template>
