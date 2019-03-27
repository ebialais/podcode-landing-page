<template>
    <div id="nav">
        <div id="navBar">
            <a @click="goAccueil1"><img :src="logo.source" :id="logo.title"/></a>
            <ul class="nav navbar-nav navbar-right nav-pills">
                <li v-for="(icon, index) in icones" :key="index">
                    <a :href="icon.lien"><i :class="icon.class"></i></a>
                </li>
                <!-- <li>
                    <a @click="goAccueil"><i  class="fas fa-home"></i></a>
                </li> -->
                <li>
                    <a id="hamburger" @click="changeBar">
                        <i v-if="bar" class="fas fa-bars" ></i>
                        <i v-else class="fas fa-times"></i>
                    </a>
                </li>
            </ul>
        </div>
        <div v-if="!bar" id="menu">
                <ul>
                    <li class="menuLi" @click="goAccueil">Accueil</li>
                    <li class="menuLi" @click="goEpisodes">Episodes</li>
                    <li class="menuLi">Blog</li>
                    <li class="menuLi">Contact</li>
                </ul>
            </div>
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
        methods: {
            // showMenu (){
            //     this.showTopMenu = !this.showTopMenu
            // },
            goAccueil1(){
                this.$router.push('/Accueil');
            },
            goAccueil(){
                this.$router.push('/Accueil');
                this.bar = !this.bar;
            },
            goEpisodes(){
                this.$router.push('/Emissions');
                this.bar = !this.bar;
            },
            changeBar(){
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

    

    #menu{
        width: 102%;
        margin: auto;
        height: 92vh;
        background-color: #96c3ca;
        font-family: 'Concert One', cursive;
        text-align: center;
        position: fixed;
         
    }


    .menuLi{
        list-style-type: none;
        font-size : 6vw;
        cursor: pointer;
        
    }
    .menuLi:hover{
        list-style-type: none;
        font-size : 6vw;
        background-color: #506f77;
        cursor: pointer;
        color: white;
        box-sizing: content-box;
        width: 100%;
    }
    
    ul {
        /* margin-left: -40px; */
        margin: 0;
        padding: 0;
    }

</style>
