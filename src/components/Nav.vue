<template>
    <div id="nav">
        <a :href="logo.lien"><img :src="logo.source" :id="logo.title"/></a>
        <ul class="nav navbar-nav navbar-right nav-pills">
            <li v-for="(icon, index) in icones" :key="index">
                <a :href="icon.lien"><i :class="icon.class"></i></a>
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
            ]
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
    .fab  {
    margin-left: -34px;
    color:#b0b9c4;
    font-size: 1.5em;
    margin-top: 13px;
    margin-right: 30px;
    -webkit-transition: all .2s ease-in-out;
    transition: all .2s ease-in-out;
}
    .fab:hover {
        color: #759faa;
        transform: scale(1.6);
        font-size: 1.5em;
        margin-right: 30px;
    }


</style>
