<template>
  <div id="app">
    <nab class="mb-4"/>
    <div class="container">
      <home/>
    </div>
  </div>
</template>

<script>
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
}
</style>
