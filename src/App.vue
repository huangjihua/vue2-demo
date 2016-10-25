<template>
  <div id="app">
    <img src="./assets/logo.png">
    <hello></hello>
    <A></A>
    <br>
    <B></B>
  </div>
</template>

<script>
import Hello from './components/Hello'
import A from './components/A'
import B from './components/B'
import store from './vuex/store'
export default {
  name: 'app',
  components: {
    Hello,
    A,
    B
  },
  store: store
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
