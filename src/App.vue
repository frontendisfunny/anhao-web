<template>
  <div id="app">
    <SecretView
    :rowtext="rowtext"
    :columntext="columntext"
    />

    <div id="button" @click="showInput">
      我也要玩
    </div>

    <div v-if="inputshow">
      <input v-model="message" placeholder="edit me">
      <input v-model="message" placeholder="edit me">
    </div>
  </div>
</template>

<script>
  import SecretView from './components/SecretView.vue'

  export default {
    name: 'App',
    components: {
      SecretView
    },
    data () {
      return {
        inputshow: false,
        rowtext: '我也不想这样反反复复',
        columntext: '反正每个人最后都孤独',
      }
    },
    methods: {
      showInput() {
        this.inputshow ? this.inputshow = false : this.inputshow = true
      },
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