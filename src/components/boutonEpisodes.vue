<template>
    <button @click="goEpisodes">Les Episodes</button>
</template>

<script>
export default {
    name: 'boutonEpisodes',
    methods: {
        goEpisodes(){
            this.$router.push('/Emissions');
        },
    }
}
</script>

<style>
button {
    text-align: center;
    margin-left: 150px;
    margin-top: 62px;
    padding: 10px 10px 10px 10px;
    color: #fff;
    font-size: 1.5em;
    text-align: center;
    -webkit-transition-duration: 0.4s; /* Safari */
    transition-duration: 0.5s;
    text-decoration: none;
    overflow: hidden;
    background-color: #69a1ac;
    border: none;
    }

button:hover {
    background-color: #69a1ac;
    -webkit-box-shadow: 0px 1px 71px 33px rgb(105, 161, 172);
    /* box-shadow: 0px 2px 59px 5px rgba(105, 161, 172, 0.64); */
    color: #ffffff;
    transform: scale(1.05);
    /* border: solid white 1px; */
}







</style>
