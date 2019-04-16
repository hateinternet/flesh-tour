<template>
  <div id="app">
    <Concerts />
  </div>
</template>

<script>
import Concerts from './components/Concerts.vue'

export default {
  name: 'app',
  components: {
    Concerts
  }
}
</script>

<style>
#app {
  font-family: Impact, Charcoal, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

@media (max-width: 1280px) {
  #app {
    margin-top: 30px;
  }
}
</style>
