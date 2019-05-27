<template>
    <div id="Accueil2" class="jumbotron-fluid">
        <div id="main">
            <h1 id="titreAccueil">{{ titre }}</h1>
            <p id="message">{{ message }}</p>
            <br />
            <p id="bannière">{{ bannière }}</p>
            <button @click.passive="goEpisodes" id="button">Episodes</button>
        </div>
        <IllustrationAccueil />
    </div>
</template>

<script>

    import IllustrationAccueil from './IllustrationAccueil.vue'

    export default {
        name: 'TextAccueil',
        components: {
            IllustrationAccueil,
        },
        data () {
            return {
                titre: 'Un podcast sur le développement web.',
                message: "Le podcast qui parle à la génération d'auto-apprenants des technologies web. Nous sommes inspirés par l'idée de dé-coder les sujets de soft-skills ou tech-skills. En bref, libérer la parole et le savoir pour accompagner le parcours de \"l'aspirant web-dev\".",
                bannière: '#Innovation, #Entrepreunariat, #MarcheDuTravail, #AutoFormation, #Productivite, #Outils.'
            }
        },
        methods: {
            goEpisodes(){
                console.log("blabla")
                this.$router.push('/Emissions');
            }
        }
    }
</script>

<style scoped>
    #main {
        position: absolute;
        width: 40%;
        top:15%;
        left:4%;
        display: flex;
        flex-flow: column nowrap;
        margin-right: 100px;
        padding-top: 80px;
        margin-left: 61px;
        z-index: 0;
    }
    #message {
        width: 100%;
        margin: 0px;
        font-size: 1em;
    }


    #bannière {
        width: 100%;
        font-size: 1em;
        margin: 0;
    }

    #button {
        width: 150px;
        color: #ffffff;
        background-color: #96c3ca;
        border-color: #96c3ca;
        transition: all .2s ease-in-out; 
        z-index: 200;
        margin-top: 46px;
        padding: 8px;
        font-size: 1.5em;
    }

    h1 {
        width: 433px;
        font-size: 39px;
        color: #96c3ca;
        font-family: 'Concert One', cursive;
        margin-bottom:45px;
    }

    p {
        font-family: 'Lato', sans-serif; 
        margin-right: 200px;
        font-size: 1.5em;
        /*margin: 100px;*/
    }

    
    @media only screen and (max-width: 800px){
        #Accueil2 {
            position: absolute;
            width: 80%;
            top: 8%;
            left:4%;
            margin-right: 0px;
            padding-top: 0px;
            display: flex;
            flex-flow: column nowrap;
        }
        #main {
            width: 100%;
            margin: 85px 20px 20px;
        }

        h1{
            width: 100%;
            margin-bottom:5px;
        }

        #message {
            width: 90%;
            /* margin: 0px; */
            font-size: 0.9em;
            /* margin-top: 20px; */
        }

        #bannière {
            width: 100%;
            font-size: 2em;
            margin: 0;
        }
        
    }


    /* @media only screen and (max-width: 400px){

        h1{
            font-size: 25px;
            margin-top: 5px;
        }
    

        #message {
            width: 100%;
            margin: 0px;
            font-size: 0.9em;
            margin-top: 15px;
        }
        
        #bannière {
            font-size: 0.8em;
        }
    } */




</style>
