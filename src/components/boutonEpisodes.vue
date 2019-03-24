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

</style>
