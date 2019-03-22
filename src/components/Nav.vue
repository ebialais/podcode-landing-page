<template>
    <div id="nav">
        <a :href="logo.lien"><img :src="logo.source" :id="logo.title"/></a>
        <!-- <quick-menu :menu-count=count :icon-class=icons :menu-url-list=list> -->
            <ul class="nav navbar-nav navbar-right nav-pills">
                <li v-for="(icon, index) in icones" :key="index">
                    <a :href="icon.lien"><i :class="icon.class"></i></a>
                </li>
                <li>
                    <a @click="goHome"><i  class="fas fa-home"></i></a>
                </li>
                <!-- <li class="menu-icon">
                    
                    <div @click="showMenu" v-if="!showTopMenu">
                        <span class="line line01"></span>
                        <span class="line line02"></span>
                        <span class="line line03"></span>
                    </div>
                    <div v-else class="openMenu-icon">
                        ✕
                    </div>
                </li> -->
            </ul>
        <!-- </quick-menu> -->
        <!-- <ul class="nav navbar-nav navbar-right nav-pills">
            <li v-for="(icon, index) in icones" :key="index">
                <a :href="icon.lien"><i :class="icon.class"></i></a>
            </li>
        </ul> -->
    </div>
</template>

<script>
    // import Vue from 'vue'
    // import quickMenu from 'vue-quick-menu'
    export default {
        name: 'NavBar', 
        // props: {
        //     menuCount: {
        //         required: true,
        //         default: 4, 
        //         type: Number,
        //     },
        //     menuUrlList: {
        //         required: true,
        //         type: Array,
        //     },
        //     iconClass: {
        //         required: true,
        //         type: Array,
        //     },
        //     position: {
        //         required: false,
        //         type: top,
        //     },
        //     backgroundColor: {
        //         required: false,
        //         default: "#009dc7", 
        //         type: String,
        //     },
        //     color: {
        //         required: false,
        //         default: "#ffffff", 
        //         type: String,
        //     },
        //     isOpenNewTab: {
        //         required: false,
        //         default: false, 
        //         type: Boolean,
        //     },
        // },
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
                showTopMenu: false,
            }
        },
        // components: {
        //     quickMenu
        // },
        methods: {
            showMenu (){
                this.showTopMenu = !this.showTopMenu
            },
            goHome(){
                this.$router.push('/');
            }
        }
    }
</script>

<style scoped>
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
        margin-right: 30px;
    }
    .menu-icon {
        width:40px;
        height:30px;
        margin-top: 40px;
        margin-right: 30px;
    }
    .line {
        position: absolute;
        height: 5px;
        width:100%;
        background:black;
        border-radius:10px;
        transition: all cubic-bezier(0.25, 0.1, 0.28, 1.54) 0.32s;
    }

    .line01 {
        top:19%;
    }

    .line02 {
        top:49%;
    }

    .line03 {
        top:79%;
    }

    

</style>
