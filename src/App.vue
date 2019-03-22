<template>
  <div id="app">
    <NavBar />
    <Accueil />
    <router-link to="/">Home</router-link>
    <router-link to="/Emissions">Les épisodes...</router-link>
    <router-view />
  </div>
  <!-- class="btn btn-primary btn" -->
</template>

<script>
  import {router} from './main.js'  
  import NavBar from './components/Nav.vue'
  import Accueil from './components/Accueil.vue'

  export default {
    name: 'app',
    components: {
      NavBar,
      Accueil,
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
