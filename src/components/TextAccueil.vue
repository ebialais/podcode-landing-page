<template>
    <div id="TextAccueil">
        <h1>{{ titre }}</h1>
        <p>{{ message }}</p>
        <button>Les épisodes...</button>
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

<style>

</style>
