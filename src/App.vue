<template>
  <div id="app">
   
    <NavBar />
    <Header />
  </div>
</template>

<script>


import NavBar from './components/NavBar.vue'
import Header from './components/Header.vue'

export default {
  name: 'app',
  components: {
    NavBar,
    Header
  }
}
</script>

<style>
#app {
 
 
}
</style>
