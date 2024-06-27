<!-- AllComponents.vue -->
<script setup>
import GettingInputValue from './GettingInputValue.vue'
import ifElse from './ifElse.vue'
import ForLoopAndList from './ForLoopAndList.vue'
import PassingDataParentToChild from './PassingDataParentToChild.vue'
import CssClassBinding from './CssClassBinding.vue'
import FormModifier from './FormModifier.vue'
import NonPropsData from './NonPropsData.vue'
</script>

<template>
  <div class="container">
    <h1>ALL COMPONENTS</h1>
    <!-- <GettingInputValue /> -->
    <!-- <ifElse /> -->
    <!-- <ForLoopAndList /> -->
    <!-- <PassingDataParentToChild /> -->
    <!-- <CssClassBinding /> -->
    <!-- <FormModifier /> -->
    <NonPropsData name="Adi" id="prop-id" />
  </div>
</template>

<style scoped>
.container {
  position: absolute;
  top: 10px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  h1 {
    font-size: 40px;
    margin-bottom: 10px;
    font-weight: bold;
    text-decoration: underline;
  }
}
</style>
