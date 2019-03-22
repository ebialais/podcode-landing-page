<template>
    <div id="Main">
        <TextAccueil />
        <IllustrationAccueil />
    </div>
</template>

<script>
    import TextAccueil from './TextAccueil.vue'
    import IllustrationAccueil from './IllustrationAccueil.vue'
    export default {
        name: 'SectionAccueil',
        components: {
            TextAccueil,
            IllustrationAccueil,
        }
    }
</script>

<style scoped>
    #Main {
        display: flex;
        margin: 100px;
    }

   

</style>
