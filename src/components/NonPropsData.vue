<script setup>
const props = defineProps({ inheritAttrs: false, name: String })
</script>

<template>
  <div>
    <div>
      <h2 v-bind="$attrs">Non Props Data</h2>
      <br />
      <h3>Madhav</h3>
      <h3>Yashu</h3>
      <h3>Aditya</h3>
      <h3>Through Props --> {{ props.name }}</h3>
    </div>
    <div>
      <div v-bind="$attrs">
        <h2>Non Props Data</h2>
        <br />
        <h3>Madhav</h3>
        <h3>Yashu</h3>
        <h3>Aditya</h3>
        <h3>Through Props --> {{ props.name }}</h3>
      </div>
    </div>
  </div>
</template>
