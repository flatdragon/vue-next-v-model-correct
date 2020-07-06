<template>
  <div id="app">
    <div>
      <h1>Vue 2 v-model behaviour</h1>
      <a href="https://github.com/flatdragon/vue-next-v-model-correct/blob/master/src/App.vue">See component source code</a>
    </div>

    <div>
      <h2>Using value with explicitly set 'undefined' value</h2>
      <div>Input value: {{ value }}</div>
      <input type="text" v-model="value">
    </div>

    <div>
      <h2>Using some state object without defining 'value' property</h2>
      <div>Input value: {{ state.value }}</div>
      <input type="text" v-model="state.value">
    </div>
  </div>
</template>

<script>
  export default {
    name: 'App',
    data () {
      return {
        value: undefined,
        state: {},
      }
    },
  }
</script>
