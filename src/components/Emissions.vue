<template>
    <div id="emissions">
        <p>Derniers épisodes</p>
        <illu2 />

       <iframe width="80%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/590494680&color=%23b6bec8&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true"></iframe>
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
