<template>
    <!-- Header Container Start  -->
    <div class="header-container">
        <div class="logo">
            <a href="/"><img src="../assets/logo.svg" alt="Logo svg"></a>
        </div>
        <div class="nav-menu">
            <a href="#about"><span>about</span></a>
            <a href="#services"><span>services</span></a>
            <a href="#portfolio"><span>portfolio</span></a>
            <a href="#contact"><span>contact</span></a>
            <a href="../assets/resume.pdf"><span>resume</span></a>
        </div>
        <div class="hamburger">
            <button @click="toggleOn"><i class="fas fa-bars"></i></button>
        </div>
        <div v-show="show" class="mobile-nav-menu">
            <a @click="toggleOff" href="#about"><span>about</span></a>
            <a @click="toggleOff" href="#services"><span>services</span></a>
            <a @click="toggleOff" href="#portfolio"><span>portfolio</span></a>
            <a @click="toggleOff" href="#contact"><span>contact</span></a>
            <a @click="toggleOff" href="../assets/resume.pdf"><span>resume</span></a>
            <button @click="toggleOff"><i class="fas fa-times"></i></button>
        </div>
    </div>
    <!-- Header Container End  -->
</template>

<script>


    export default {
        name: 'Header',
        data(){
            return{
                show: false,
            }
        },
        methods:{
            toggleOn(){
                this.show = true
                document.body.classList.add('no-scroll')
            },
            toggleOff(){
                this.show = false
                document.body.classList.remove('no-scroll')
            },
            samir(){
                const body = document.body
                this.show ? body.classList.add('no-scroll') : body.classList.remove('no-scroll')
            }
        },
    }
</script>

<style scoped>
    .header-container{
        position: relative;
        width: 100%;
        padding: 4rem 8rem;
        display: flex;
        justify-content: space-between;
        align-items: center;
        position: absolute;
        top: 0;
        left: 0;
    }
    .logo{
        width: 15rem;
        position: relative;
    }
    .logo img{
        width: 100%;
    }
    .nav-menu{
        position: relative;
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        align-items: center;
    }
    .nav-menu a{
        display: inline-block;
        margin: 1rem;
        text-decoration: none;
        color: var(--font-dark);
    }
    .nav-menu a span{
        font-size: 2rem;
        text-transform: capitalize;
        padding: 1rem 2rem;
        background: var(--accent-1);
        border-radius: 2rem;
    }
    .nav-menu a:last-child span{
        background: var(--accent-2);
    }
    .nav-menu a:hover span{
        box-shadow: 0 0 2rem var(--accent-1-50);
    }
    .nav-menu a:last-child:hover span{
        box-shadow: 0 0 2rem var(--accent-2-50);
    }
    .mobile-nav-menu{
        position: fixed;
        width: 100%;
        height: 100%;
        top: 0;
        left: 0;
        display: flex;
        flex-direction: column;
        padding: 4rem;
        justify-content: center;
        align-items: center;
        z-index: 9999;
        background: var(--bg-dark);
    }
    .mobile-nav-menu button{
        font-size: 3rem;
        border: none;
        background: none;
        color: var(--accent-2);
        position: absolute;
        top: 5%;
        left: 5%;
    }
    .mobile-nav-menu a{
        font-size: 2rem;
        margin: 1rem;
        text-decoration: none;
        color: var(--accent-2);
        text-transform: uppercase;
    }
    .mobile-nav-menu a:last-child{
        color: var(--accent-1);
    }
    .hamburger{
        display: none;
    }
    @media screen and (max-width: 1200px){
        .header-container{
            padding: 1rem 2rem;
            justify-content: space-between;
        }
        .nav-menu a span{
            font-size: 1.3rem;
        }
    }
    @media screen and (max-width: 992px){
        .header-container{
            padding: 1rem 2rem;
            justify-content: space-between;
        }
        .nav-menu a span{
            font-size: 1.3rem;
        }
    }
    @media screen and (max-width: 768px) {
        .header-container{
            padding: 1rem 2rem;
            justify-content: space-between;
        }
        .header-container .logo{
            width: 10rem;
        }
        .header-container .nav-menu{
            display: none;
        }
        .header-container .hamburger{
            padding: 2rem;
            display: block;
        }
        .header-container .hamburger button{
            background: none;
            color: var(--accent-2);
            border: none;
            font-size: 3rem;

        }
    }
    @media screen and (max-width: 576px) {
        .header-container{
            padding: 1rem 2rem;
            justify-content: space-between;
        }
        .header-container .logo{
            width: 10rem;
        }
        .header-container .nav-menu{
            display: none;
        }
        .header-container .hamburger{
            padding: 2rem;
            display: block;
        }
        .header-container .hamburger button{
            background: none;
            color: var(--accent-2);
            border: none;
            font-size: 3rem;

        }
    }

</style>