<template>
  <div id="app">
    <SecretView />
  </div>
</template>

<script>
  import SecretView from './components/SecretView.vue'

  export default {
    name: 'App',
    components: {
      SecretView
    }
  }
</script>

<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
  }
</style>