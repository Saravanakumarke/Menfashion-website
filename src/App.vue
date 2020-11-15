<template>
  <div id="app">
    
    <menfashion />
  </div>
</template>

<script>

import Menfashion from './components/Menfashion.vue'

export default {
  name: 'App',
  components: {
   
    Menfashion
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
}
</style>
