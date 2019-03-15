<template>
  <div id="app">
    <NavBar />
    <SectionAccueil />
    <Illustration />
  </div>
</template>

<script>
  import NavBar from './components/Nav.vue'
  import SectionAccueil from './components/SectionAccueil.vue'
  import Illustration from './components/Illustration.vue'

  export default {
    name: 'app',
    components: {
      NavBar,
      SectionAccueil,
      Illustration,
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
