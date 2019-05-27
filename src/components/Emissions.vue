<template>
    <div id="emissions">
      <div id="episodes">
        <p>Derniers épisodes</p>
        <ChoixEpisodes />
      </div>
        <illu2 />
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
    z-index: 0;
    border-radius: 10px;
    display: flex;
    flex-flow: column nowrap;
  }

  #emissions:hover {
    box-shadow: 0 0 11px rgba(3, 53, 148, 0.2); 
  }

  p {
    font-size: 0.5em;
    margin-top: 15px;
  }
  @media only screen and (max-width: 800px){
    #emissions {
      display: flex;
      flex-flow: column nowrap;
      width: 100%;
      margin: -90px -17px;
      background-color: #fff;
      box-shadow: none;
      height: fit-content;
      overflow-y: auto;
    }
    #episodes{
      width: 80%;
      margin: auto;
    }
      
  }
</style>
