<template>
    <div id="nav">
        <a @click="goAccueil"><img :src="logo.source" :id="logo.title"/></a>
        <ul class="nav navbar-nav navbar-right nav-pills">
            <li v-for="(icon, index) in icones" :key="index">
                <a :href="icon.lien"><i :class="icon.class"></i></a>
            </li>
            <!-- <li>
                <a @click="goAccueil"><i  class="fas fa-home"></i></a>
            </li> -->
            <li>
                <a @click="goMenu">
                    <i v-if="bar" class="fas fa-bars"></i>
                    <i v-else class="fas fa-times"></i>
                </a>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: 'NavBar', 
        data (){
            return {
                logo: {
                    title: 'podcode',
                    source: './assets/logo_podcode_black.png',
                    lien: '#',
                },
                icones: [
                    {title: 'soundCloud', lien:'#', class: 'fab fa-soundcloud'},
                    {title: 'facebook', lien:'#', class: 'fab fa-facebook-f'},
                    {title: 'twitter', lien:'#', class: 'fab fa-twitter'}, 
                ],
                bar: true,
            }
        },
        // components: {
        //     quickMenu
        // },
        methods: {
            showMenu (){
                this.showTopMenu = !this.showTopMenu
            },
            goAccueil(){
                this.$router.push('/Accueil');
            },
            goMenu(){
                this.$router.push('/Menu');
                this.bar = !this.bar;
            }
        }
    }
</script>

<style scoped>
    #nav {
        width: 98.5vw;
    }
    #podcode {
        width: 9vw;
        margin-left: 2vw;
        margin-top: 7px;
        }
    .nav>li>a:hover, .nav>li>a:focus {
        text-decoration: none;
        background-color: transparent;
    }
    .fab, .fas  {
    margin-left: -34px;
    color:#b0b9c4;
    font-size: 1.5em;
    margin-top: 13px;
    margin-right: 30px;
    -webkit-transition: all .2s ease-in-out;
    transition: all .2s ease-in-out;
    }
    .fab:hover, .fas:hover {
        color: #759faa;
        transform: scale(1.6);
        font-size: 1.5em;
        margin-right: 27px;
    }

    

</style>
