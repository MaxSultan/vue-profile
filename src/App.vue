<template>
  <div id="app">
    <navBar/>
    <home/>
    <tech/>
  </div>
</template>

<script>
import home from './components/home.vue'
import tech from './components/tech.vue'
import navBar from './components/navBar.vue'

export default {
  name: 'App',
  components: {
    home,
    tech,
    navBar
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
.frame{
    height: 100vh;
    width: 100vw;
}
*{
  margin: 0;
  padding: 0;
}
</style>
