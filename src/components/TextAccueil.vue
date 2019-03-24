<template>
    <div id="TextAccueil" class="jumbotron-fluid">
        <h1>{{ titre }}</h1>
        <p>{{ message }}</p>
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
        },
    }
</script>

<style scoped>
    #TextAccueil {
        width: 50%;
        display: flex;
        flex-flow: column nowrap;
        margin-right: 100px;
        padding-top: 120px;
        margin-left: 61px;
        
    }
    .btn {
        width: 150px;
        color: #ffffff;
        background-color: #96c3ca;
        border-color: #96c3ca;
        transition: all .2s ease-in-out; 
    }
    .btn:hover {
        color: #ffffff;
        background-color: #759faa;
        border-color: #759faa;
    }
    h1 {
        width: 433px;
        font-size: 39px;
        color: #96c3ca;
        font-family: 'Concert One', cursive;


    }
    p{
        font-family: 'Lato', sans-serif; 
        margin-right: 200px;
        font-size: 1.5em;

        /*margin: 100px;*/
    }


button {
    position: relative;
    background-color: #69a1ac;
    border: none;
    padding: 4px;
    width: 200px;
    color: #fff;
    font-size: 1.5em;
    text-align: center;
    -webkit-transition-duration: 0.4s; /* Safari */
    transition-duration: 0.5s;
    text-decoration: none;
    overflow: hidden;
    margin-left: 60px;
    margin-top: 20px;
}

button:hover{
   background: #c1dee2;
    -webkit-box-shadow: 0px 2px 10px 5px rgb(11, 82, 121);
    box-shadow: 0px 2px 10px 5px rgb(193, 222, 226);
    color: #191847;
}



button:after {
    content: "";
    background: #89c5cc;
    display: block;
    position: absolute;
    padding-top: 300%;
    padding-left: 350%;
    margin-left: -20px !important;
    margin-top: -120%;
    opacity: 0;
    transition: all 0.8s
}

button:active:after {
    padding: 0;
    margin: 0;
    opacity: 1;
    transition: 0s
}



</style>
