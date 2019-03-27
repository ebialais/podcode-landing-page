<template>
    <div id="footer">
        <img src="assets/creative-commons-783531_960_720.png">
        <p> | 2019 | Un projet issu de BeCode | Design du site web par Andres Goldestein & Emilie Bialais</p>
    </div>
</template>

<script>
    export default {
        name:'pied',
    }
</script>

<style>

    #footer {
        display: flex;
        justify-content: center; 
        align-items: center;
        position: fixed;
        left: 0px;
        top:780px;
        width: 100%;
        background-color: #f2f2f2;
        height: 40px;
        text-align: center;
        z-index: -1;
        
}
    img {
        width: 70px;
        margin-right: 25px;
    
    }

    #footer p {
        font-size: 0.8em;
        margin-top: 12px;
        color: #303777;
    }

</style>
