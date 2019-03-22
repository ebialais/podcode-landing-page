<template>
    <div id="TextAccueil" class="jumbotron-fluid">
        <h1>{{ titre }}</h1>
        <p>{{ message }}</p>
        <!-- <router-link to="/Emissions" class="btn btn-primary btn">Les épisodes...</router-link>
        <router-view /> -->
    </div>
</template>

<script>
    export default {
        name: 'TextAccueil',
        data () {
            return {
                titre: 'Bienvenue à Podcode',
                message: 'SoundCloud is a music and podcast streaming platform that lets you listen to millions of songs from around the world, or upload your own. Start listening now!',
            }
        }
    }
</script>

<style scoped>
    #TextAccueil {
        width: 50%;
        display: flex;
        flex-flow: column nowrap;
        
    }
    .btn {
        width: 150px;
        color: #ffffff;
        background-color: #96c3ca;
        border-color: #96c3ca;
        transition: all .2s ease-in-out; 
    }
    .btn:hover {
        color: #ffffff;
        background-color: #759faa;
        border-color: #759faa;
    }
    h1 {
        width: 433px;
        font-size: 39px;
        color: #96c3ca;
        font-family: 'Concert One', cursive;


    }
    p{
        font-family: 'Lato', sans-serif; 

        /*margin: 100px;*/
    }

</style>
