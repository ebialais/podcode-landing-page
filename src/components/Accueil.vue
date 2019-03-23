<template>
    <div id="Main">
        <div class="text">
            <TextAccueil id="TextAccueil" />
            <boutonEpisodes id="boutonEpisodes" />
        </div>
        <IllustrationAccueil id="IllustrationAccueil" />
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
        margin: 80px;
    }
    #TextAccueil {
        display: init;
    }
    #boutonEpisodes {
        display: init;
    }
    #IllustrationAccueil {
        display: init;
    }
</style>
