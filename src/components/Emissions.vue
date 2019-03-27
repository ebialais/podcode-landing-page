<template>
    <div id="emissions">
        <p>Derniers épisodes</p>
        <illu2 />
        <ChoixEpisodes />
    </div>
</template>

<script>
  import ChoixEpisodes from './ChoixEpisodes.vue'
  import illu2 from './illu2.vue'
  
  export default {
    components : {
      ChoixEpisodes,
      illu2,
    }
  }
</script>

<style>
  #emissions {
    width: 47vw;
    height: 68vh;
    background-color: #89c5ccda;
    position: absolute;
    top: 20%;
    left: 5%;
    color:rgb(35, 35, 85);
    font-size: 2em;
    text-align: center;
    box-shadow: 0 0 11px rgba(33,33,33,.2); 
    transition: box-shadow .3s;
    z-index: -50;
    border-radius: 10px;
  }

  #emissions:hover {
    box-shadow: 0 0 11px rgba(3, 53, 148, 0.2); 
  }

  p {
    font-size: 0.5em;
    margin-top: 15px;
  }

</style>
