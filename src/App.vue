<template>
  <div id="app">
    <NavBar />
    <router-view />
  </div>
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
  }
</style>
