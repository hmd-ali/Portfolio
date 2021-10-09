<template>
    <!-- Pre-Loader Container Start  -->
    <transition name="fade">
        <div v-if="!isLoaded" class="pre-loader">
            <img ref="animation" src="../assets/logo.svg" alt="PreLoader Animation">
            <div class="made-by"><h1>Made with love...</h1></div>
            <div class="dots">
                <div class="dot animation-left"></div>
                <div class="dot"></div>
                <div class="dot"></div>
                <div class="dot"></div>
                <div class="dot"></div>
                <div class="dot animation-right"></div>
            </div>
        </div>
    </transition>
    <!-- Pre-Loader Container End  -->
</template>

<script>

    export default {
        name: 'PreLoader',
        data(){
            return{
                isLoaded: false,
            }
        },
        mounted(){
            document.body.classList.add('no-scroll')
            document.onreadystatechange = () => {
                if( document.readyState == 'complete'){
                    document.body.classList.remove('no-scroll')
                    this.isLoaded = true // Code to hide pre-loader
                }
            }
        }
    }
</script>

<style scoped>
    .pre-loader{
        position: fixed;
        z-index: 99999;
        width: 100vw;
        height: 100vh;
        background: var(--bg-dark);
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
    .pre-loader img{
        width: 20rem;
        height: 20rem;
        padding: 1rem 1rem;
    }
    .pre-loader .made-by{
        padding: 2rem;
    }
    .pre-loader .made-by h1{
        color: var(--accent-2);
        font-weight: 300;
    }
    .pre-loader .dots{
        padding: 2rem;
        position: relative;
        display: flex;
    }
    .pre-loader .dots .dot{
        width: 1rem;
        height: 1rem;
        margin: 1rem;
        background: var(--accent-2);
    }
    .animation-left{
        animation: left 1s infinite;
    }
    .animation-right{
        animation: right 1s infinite .5s;
    }
    @keyframes left {
        40%{
            transform: translateX(-2rem);
        }
        50%{
            transform: translateX(0rem);
        }
    }
    @keyframes right {
        40%{
            transform: translateX(2rem);
        }
        50%{
            transform: translateX(0rem);
        }
    }
    @media screen and (max-width: 576px) {
        .pre-loader img{
            width: 15rem;
            height: 15rem;
        }
    }
    
</style>