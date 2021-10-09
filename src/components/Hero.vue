<template>
    <!-- Hero Container Start  -->
    <div class="hero-container" id="hero">
        <Header />
        <div class="content-container">
            <h2>Howdy, I am</h2>
            <h1>
                Ali Hammoud,<br>
                <span>and I love coding.</span>
            </h1>
            <a href="#about" class="more-about-me"><span>More About Me</span></a>
        </div>
        <div class="illustration">
            <img src="../assets/undraw.svg" alt="">
        </div>
    </div>
    <!-- Hero Container End  -->
</template>

<script>

    import Header from './Header.vue'

    export default {
        name: 'Hero',
        components:{
            Header,
        },
        
    }
</script>

<style scoped>
    .hero-container{
        position: relative;
        width: 100%;
        height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
    .illustration{
        position: absolute;
        top: 50%;
        right: 0;
        width: 50%;
        height: 100%;
        transform: translateY(-50%);
        display: flex;
        align-items: center;
        justify-content: center;
        z-index: -1;
    }
    .illustration img{
        width: 100%;
        padding: 2rem;
    }
    .content-container{
        position: relative;
        width: 50%;
        padding: 4rem 8rem;
        overflow: hidden;
    }
    .content-container h2{
        color: var(--accent-1);
        opacity: .8;
        font-size: 2rem;
        margin-bottom: 2rem;
    }
    .content-container h1{
        font-size: 5rem;
        color: var(--font-light);
    }
    .content-container h1 span{
        opacity: .5;
    }
    .more-about-me{
        display: inline-block;
        text-decoration: none;
        color: var(--font-dark);
        font-size: 1.5rem;
        font-weight: 600;
        margin-top: 3rem;
    }
    .more-about-me span{
        padding: 1rem 2rem;
        background: var(--accent-2);
        border-radius: 2rem;
        position: relative;
        overflow: hidden;

    }
    .more-about-me:hover span{
        background: var(--accent-1-50);
    }
    .background-animations{
        position: absolute;
        width: 100%;
        height: 100%;
    }
    .background-animations .polygon{
        position: relative;
    }
    .background-animations .circle{
        position: absolute;
        top: 30%;
        right: 54%;
        width: 5rem;
        height: 5rem;
        border-radius: 50%;
         background: var(--accent-2);
    }
    .background-animations .circle::before{
        content: '';
        position: absolute;
        width: 100%;
        height: 100%;
        top: 2rem;
        left: -1rem;
        border-radius: 50%;
        background: var(--accent-2);
        opacity: .5;
    }
    @media screen and (max-width: 768px) {
        .hero-container{
            justify-content: center;
        }
        .hero-container .illustration{
            position: unset;
            width: 100%;
            height: unset;
            top: unset;
            left: unset;
            transform: translate(0,0);
        }
        .hero-container .content-container{
            width: 100%;
            margin-top: 10rem;
            padding: 1rem 2rem;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
        .hero-container .content-container h2{
            font-size: 1rem;
        }
        .hero-container .content-container h1{
            font-size: 2rem;
        }
    }
    @media screen and (max-width: 576px) {
        .hero-container{
            justify-content: center;
        }
        .hero-container .illustration{
            position: unset;
            width: 100%;
            height: unset;
            top: unset;
            left: unset;
            transform: translate(0,0);
        }
        .hero-container .content-container{
            width: 100%;
            margin-top: 10rem;
            padding: 1rem 2rem;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }
        .hero-container .content-container h2{
            font-size: 1rem;
        }
        .hero-container .content-container h1{
            font-size: 2rem;
        }
    }
</style>