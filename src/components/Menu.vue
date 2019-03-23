<template>
    <div id="menu">
        <ul>
            <li @click="goAccueil">Home</li>
            <li @click="goEpisodes">Episodes</li>
            <li>Blabla</li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'menu',
    methods: {
        goAccueil(){
            this.$router.push('/Accueil');
        },
        goEpisodes(){
            this.$router.push('/Emissions');
        },
    }
}
</script>

<style scoped>
    #menu{
        width: 100vw;
        height: 98vh;
        background-color: #96c3ca;
        font-family: 'Concert One', cursive;
        text-align: center;
    }
    li {
        list-style-type: none;
        font-size : 6vw;
    }

</style>
