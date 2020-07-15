<template>
  <div id="app">
    <nab/>
    <home/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import nab from './components/nav.vue'
import home from './components/home.vue'

export default {
  name: 'App',
  components: {
    nab,home
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
