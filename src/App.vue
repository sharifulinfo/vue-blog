<template>
  <div id="app">
    <nab/>
    <div class="container">
      <home/> 
      <sliders>
          <slide></slide>
      </sliders>
    </div>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import nab from './components/nav.vue'
import home from './components/home.vue'
import sliders from './components/sliders.vue'

export default {
  name: 'App',
  components: {
    nab,home,sliders
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
