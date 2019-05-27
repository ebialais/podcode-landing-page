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
  import Accueil2 from './components/Accueil2.vue'
  import pied from './components/Footer.vue'

  export default {
    name: 'app',
    components: {
      NavBar,
      Accueil2,
      pied
    },
    methods: {
      beforeLoad(){
        this.$router.push('/Accueil2');
      },
      mounted(){
        this.$nextTick(this.beforeLoad)
      }
    },
  }
</script>

<style>
  body {
    overflow-y: auto;
    overflow-x: hidden;
    width: 100vw;
    height: 100vh;
  }
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    color: #2c3e50;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 100%;
    width: 100%;
  }
</style>
