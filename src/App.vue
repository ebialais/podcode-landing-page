<template>
  <div id="app">
    <NavBar />
    <router-view />
    <pied />
  </div>
</template>

<script>
  import {router} from './main.js'  
  import NavBar from './components/Nav.vue'
  import Accueil from './components/Accueil.vue'
  import pied from './components/Footer.vue'

  export default {
    name: 'app',
    components: {
      NavBar,
      Accueil,
      pied
    },
    methods: {
      beforeLoad(){
        this.$router.push('/Accueil');
      },
    },
    mounted(){
      this.$nextTick(this.beforeLoad)
    }
  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    overflow-x: hidden;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 100vh;
  }
</style>
