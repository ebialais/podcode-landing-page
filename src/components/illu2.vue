<template>
    <div id="illu2">
        <img id="decor" src="assets/Home@2x.png" width="100%" class="img-fluid" alt="humaaans by Pablo Stanley">
        <img id="homme" src="assets/sitting-2@2x.png" width="100%" class="img-fluid" alt="humaaans by Pablo Stanley">
        <img id="femme" src="assets/standing-6.png" width="100%" class="img-fluid" alt="humaaans by Pablo Stanley">
        <img id="mic" src="assets/new_mic.png" width="100%" class="img-fluid" alt="humaaans by Pablo Stanley">
        <div>
            <p  id="pablo">@pablostanley</p>
        </div>    
    </div>
</template>

<script>
    export default {
        name: 'illu2',
    }
</script>

<style scoped>
    #homme {
        position: fixed;
        width: 13%;
        top:55%;
        left: 72%;
        animation: animationFemme ease-in-out 1s;
        animation-iteration-count: 1;
        transform-origin: 50% 50%;
        animation-fill-mode:forwards; /*when the spec is finished*/
        -webkit-animation: animationFemme  ease-in-out 2s;
        -webkit-animation-iteration-count: 1;
        -webkit-transform-origin: 50% 50%;
        -webkit-animation-fill-mode:forwards; /*Chrome 16+, Safari 4+*/ 
        -moz-animation: animationFemme  ease-in-out 2s;
        -moz-animation-iteration-count: 1;
        -moz-transform-origin: 50% 50%;
        -moz-animation-fill-mode:forwards; /*FF 5+*/
        -o-animation: animationFemme  ease-in-out 2s;
        -o-animation-iteration-count: 1;
        -o-transform-origin: 50% 50%;
        -o-animation-fill-mode:forwards; /*Not implemented yet*/
        -ms-animation: animationFemme  ease-in-out 2s;
        -ms-animation-iteration-count: 1;
        -ms-transform-origin: 50% 50%;
        -ms-animation-fill-mode:forwards; /*IE 10+*/
        z-index: -50;
        }

    @keyframes animationFemme{
        0% {
        transform:  translate(348px,40px)  ;
        }
        100% {
        transform:  translate(65px,32px)  ;
        }
    }
    
    @-moz-keyframes animationFemme{
        0% {
        -moz-transform:  translate(348px,40px)  ;
        }
        100% {
        -moz-transform:  translate(65px,32px)  ;
        }
    }
    
    @-webkit-keyframes animationFemme{
        0% {
        -webkit-transform:  translate(348px,40px)  ;
        }
        100% {
        -webkit-transform:  translate(65px,32px)  ;
        }
    }

    @-o-keyframes animationFemme {
        0% {
        -o-transform:  translate(348px,40px)  ;
        }
        100% {
        -o-transform:  translate(65px,32px)  ;
        }
    }
    
    @-ms-keyframes animationFemme{
        0% {
        -ms-transform:  translate(348px,40px)  ;
        }
        100% {
        -ms-transform:  translate(65px,32px)  ;
        }
    }
    #femme {
        position: fixed;
        width: 12%;
        top: 56%;
        left: 63%;
        animation: animationFrames ease 2s;
        animation-iteration-count: 1;
        transform-origin: 50% 50%;
        animation-fill-mode: forwards;
        -webkit-animation: animationFrames ease 2s;
        -webkit-animation-iteration-count: 1;
        -webkit-transform-origin: 50% 50%;
        -webkit-animation-fill-mode: forwards;
        -moz-animation: animationFrames ease 2s;
        -moz-animation-iteration-count: 1;
        -moz-transform-origin: 50% 50%;
        -moz-animation-fill-mode: forwards;
        -o-animation: animationFrames ease 2s;
        -o-animation-iteration-count: 1;
        -o-transform-origin: 50% 50%;
        -o-animation-fill-mode: forwards;
        -ms-animation: animationFrames ease 2s;
        -ms-animation-iteration-count: 1;
        -ms-transform-origin: 50% 50%;
        -ms-animation-fill-mode: forwards;
        z-index: -50;
    }


    @keyframes animationFrames{
        0% {
            opacity:0;
            transform:  translate(-1500px,0px)  ;
        }
        60% {
            opacity:1;
            transform:  translate(30px,0px)  ;
        }
        80% {
            transform:  translate(-10px,0px)  ;
        }
        100% {
            opacity:1;
            transform:  translate(0px,0px)  ;
        }
    }

    @-moz-keyframes animationFrames{
        0% {
        opacity:0;
        -moz-transform:  translate(-1500px,0px)  ;
        }
        60% {
        opacity:1;
        -moz-transform:  translate(30px,0px)  ;
        }
        80% {
        -moz-transform:  translate(-10px,0px)  ;
        }
        100% {
        opacity:1;
        -moz-transform:  translate(0px,0px)  ;
        }
    }

    @-webkit-keyframes animationFrames {
        0% {
        opacity:0;
        -webkit-transform:  translate(-1500px,0px)  ;
        }
        60% {
        opacity:1;
        -webkit-transform:  translate(30px,0px)  ;
        }
        80% {
        -webkit-transform:  translate(-10px,0px)  ;
        }
        100% {
        opacity:1;
        -webkit-transform:  translate(0px,0px)  ;
        }
    }

    @-o-keyframes animationFrames {
        0% {
        opacity:0;
        -o-transform:  translate(-1500px,0px)  ;
        }
        60% {
        opacity:1;
        -o-transform:  translate(30px,0px)  ;
        }
        80% {
        -o-transform:  translate(-10px,0px)  ;
        }
        100% {
        opacity:1;
        -o-transform:  translate(0px,0px)  ;
        }
    }
    
    @-ms-keyframes animationFrames {
        0% {
        opacity:0;
        -ms-transform:  translate(-1500px,0px)  ;
        }
        60% {
        opacity:1;
        -ms-transform:  translate(30px,0px)  ;
        }
        80% {
        -ms-transform:  translate(-10px,0px)  ;
        }
        100% {
        opacity:1;
        -ms-transform:  translate(0px,0px)  ;
        }
    }

    #illustration {
        width: 50%;
        height: 500px;
        opacity: 1;
    }

    #decor {
        position: fixed;
        width: 33%;
        top: 21%;
        left: 59%;
        z-index: -9999;
    }

    #mic {
        position: fixed;
        width: 3%;
        top: 57%;
        left: 73%;
        animation: animationMic 5s;
        animation-iteration-count: 1;
        transform-origin: 50% 50%;
        animation-fill-mode:forwards; /*when the spec is finished*/
        -webkit-animation: animationMic ease 5s;
        -webkit-animation-iteration-count: 1;
        -webkit-transform-origin: 50% 50%;
        -webkit-animation-fill-mode:forwards; /*Chrome 16+, Safari 4+*/ 
        -moz-animation: animationMic ease 5s;
        -moz-animation-iteration-count: 1;
        -moz-transform-origin: 50% 50%;
        -moz-animation-fill-mode:forwards; /*FF 5+*/
        -o-animation: animationMic ease 5s;
        -o-animation-iteration-count: 1;
        -o-transform-origin: 50% 50%;
        -o-animation-fill-mode:forwards; /*Not implemented yet*/
        -ms-animation: animationMic ease 5s;
        -ms-animation-iteration-count: 1;
        -ms-transform-origin: 50% 50%;
        -ms-animation-fill-mode:forwards; /*IE 10+*/
        z-index: 50;
    }

    @keyframes animationMic{
        0% {
        opacity:0;
        transform:  translate(10px,-253px)  ;
        }
        100% {
        opacity:1;
        transform:  translate(10px,0px)  ;
        }
    }

    @-moz-keyframes animationMic{
        0% {
        opacity:0;
        -moz-transform:  translate(10px,-253px)  ;
        }
        100% {
        opacity:1;
        -moz-transform:  translate(10px,0px)  ;
        }
    }

    @-webkit-keyframes animationMic {
        0% {
        opacity:0;
        -webkit-transform:  translate(10px,-253px)  ;
        }
        100% {
        opacity:1;
        -webkit-transform:  translate(10px,0px)  ;
        }
    }
    
    @-o-keyframes animationMic {
        0% {
        opacity:0;
        -o-transform:  translate(10px,-253px)  ;
        }
        100% {
        opacity:1;
        -o-transform:  translate(10px,0px)  ;
        }
    }
    
    @-ms-keyframes animationMic {
        0% {
        opacity:0;
        -ms-transform:  translate(10px,-253px)  ;
        }
        100% {
        opacity:1;
        -ms-transform:  translate(10px,0px)  ;
        }
    }

    #pablo {
        position: fixed;
        top: 59%;
        left: 89%;
        font-size: 9px;
        text-align: right;
        -webkit-writing-mode: vertical-rl;
        -ms-writing-mode: tb-rl;
        writing-mode: vertical-rl;
        text-orientation: mixed;
        z-index: 50;
    }
</style>
