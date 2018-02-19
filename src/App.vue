<template>
  <div id="app">
    <img src="./assets/logo.png" />
    <Assignment2 />
  </div>
</template>

<script>
import Assignment2 from './components/Assignment2'

export default {
  name: 'App',
  components: {
    Assignment2
  }
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
