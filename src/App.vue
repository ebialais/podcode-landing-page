<template>
  <div id="app">
    <NavBar />
    <Main />
  </div>
</template>

<script>
  import NavBar from './components/Nav.vue'
  import Main from './components/Main.vue'

  export default {
    name: 'app',
    components: {
      NavBar,
      Main,
    }
  }
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
