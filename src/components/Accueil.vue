<template>
    <div id="Main">
        <div id="text">
            <TextAccueil />
            <boutonEpisodes />
        </div>
        <IllustrationAccueil />
    </div>
</template>

<script>
    import TextAccueil from './TextAccueil.vue'
    import IllustrationAccueil from './IllustrationAccueil.vue'
    import boutonEpisodes from './boutonEpisodes.vue'
    
    export default {
        name: 'SectionAccueil',
        components: {
            TextAccueil,
            IllustrationAccueil,
            boutonEpisodes,
        },
    }
</script>

<style scoped>
    #Main {
        display: flex;
        flex-direction: row;
        /* margin: 8vw; */
        z-index:-50;
    }
    #text {
        width: 50vw;
    }
    
    @media only screen and (max-width: 800px){
        #Main {
            flex-direction: column-reverse
        }
        #text {
            width: 100vw;
        }
        
    }
</style>
