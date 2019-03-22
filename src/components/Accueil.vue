<template>
    <div id="Main">
        <TextAccueil />
        <Illustration />
    </div>
</template>

<script>
    import TextAccueil from './TextAccueil.vue'
    import Illustration from './Illustration.vue'
    export default {
        name: 'SectionAccueil',
        components: {
            TextAccueil,
            Illustration,
        }
    }
</script>

<style scoped>
    #Main {
        display: flex;
        margin: 100px;
    }

   

</style>
