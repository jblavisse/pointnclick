<template>
  <div id="app">
    <Enemies/>
  </div>
</template>

<script>
import Enemies from './components/Enemies.vue'

export default {
  name: 'app',
  components: {
    Enemies
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
