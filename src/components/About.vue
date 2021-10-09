<template>
    <!-- About Container Start  -->
    <div class="about-container" id="about">
        <div class="title">
            <h2>main info</h2>
            <h1>about me</h1>
        </div>
        <div class="content-container">
            <div class="memoji">
                <img src="../assets/memoji.png" alt="Memoji Image">
                <div class="social-links">
                    <a target="_blank" title="Facebook" href="https://www.facebook.com/ali.hammoud.35728466/"><i class="fab fa-facebook-f"></i></a>
                    <a target="_blank" title="Instagram" href="https://www.instagram.com/alihammoud77/"><i class="fab fa-instagram"></i></a>
                    <a target="_blank" title="Twitter" href="https://twitter.com/hmdali99"><i class="fab fa-twitter"></i></a>
                    <a target="_blank" title="Github" href="https://github.com/hmd-ali"><i class="fab fa-github"></i></a>
                </div>
            </div>
            <div class="content">
                <div class="about-me">
                    <p>Thank you for checking out my website! <span>I'm Ali Hammoud, and I'm a self-taught Lebanese developer. </span>I've always been the computer guy since I was a kid, but didn't really pick up coding until I was 16 years old-but then, oh boy I was hooked!</p>
                    <p>I started coding programs that would automate my playing online games, but eventually I dropped that altogether, and that love for video games transferred over to programming. I've been coding non-stop since.</p>
                </div>
                <div class="links">
                    <a href="../assets/resume.pdf">download cv</a>
                    <a href="mailto:letsmailali.h@gmail.com">hire me</a>
                </div>
            </div>

        </div>
    </div>
    <!-- About Container End  -->
</template>

<script>
    export default {
        name: 'About',
    }
</script>

<style scoped>
    .about-container{
        position: relative;
        width: 100%;
        margin: 15rem 0;
    }
    .about-container .title{
        width: 100%;
        position: relative;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-bottom: 10rem;
    }
    .about-container .title h2{
        font-size: 3rem;
        color: var(--accent-1);
        text-transform: uppercase;
    }
    .about-container .title h1{
        font-size: 5rem;
        color: var(--accent-2);
        text-transform: uppercase;
    }
    .about-container .content-container{
        position: relative;
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .about-container .content-container .memoji{
        position: relative;
        width: 50%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }
    .about-container .content-container .memoji img{
        width: 50%;
    }
    .about-container .content-container .memoji .social-links{
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .about-container .content-container .memoji .social-links a{
        display: inline-block;
        margin: 2rem;
        font-size: 5rem;
        text-decoration: none;
        color: var(--accent-2);
        transition: all 300ms ease;
    }
    .about-container .content-container .memoji .social-links a:hover{
        transform: translateY(-1rem) scale(.9);
        color: var(--accent-2-50);
    }
    .about-container .content-container .memoji .social-links a i{
        text-shadow: 10px 10px 1px rgba(0, 0, 0, 0.4);
    }
    .about-container .content-container .content{
        position: relative;
        width: 50%;
        display: flex;
        flex-direction: column;
        justify-content: left;
    }
    .about-container .content-container .content .about-me{
        margin-bottom: 4rem;
    }
    .about-container .content-container .content .about-me p{
        font-size: 1.8rem;
        color: var(--font-light);
        max-width: 60rem;
        text-align: justify;
        line-height: 2;
        margin: 3rem;
        margin-left: 0;
    }
    .about-container .content-container .content .links{
        position: relative;
        width: 100%;
        
    }
    .about-container .content-container .content .links a{
        display: inline-block;
        color: var(--font-dark);
        padding: 1rem 2rem;
        background: var(--accent-1);
        border-radius: 2rem;
        font-size: 2rem;
        text-decoration: none;
        margin: 1rem;
        text-transform: capitalize;
    }
    .about-container .content-container .content .links a{
        margin-left: 0;
    }
    @media screen  and (max-width: 768px){
        .about-container{
            margin: 5rem 0;
        }
        .about-container .title h2{
            font-size: 1.5rem;
        }
        .about-container .title h1{
            font-size: 3rem;
        }
        .about-container .title{
            margin-bottom: 5rem;
        }
        .about-container .content-container{
            flex-direction: column-reverse;
            padding: 1rem 2rem;
        }
        .about-container .content-container .memoji{
            margin-top: 4rem;
        }
        .about-container .content-container .memoji img{
            width: 100%;
        }
        .about-container .content-container .memoji .social-links a{
            font-size: 3rem;
        }
        .about-container .content-container .content{
            width: 100%;
        }
        .about-container .content-container .content .about-me p{
            font-size: 1.3rem;
        }
        .about-container .content-container .content .about-me{
            margin-bottom: 2rem;
        }
        .about-container .content-container .content .links{
            background: transparent;
        }
        .about-container .content-container .content .links a{
            font-size: 1.3rem;
            font-weight: 600;
        }
    }
    @media screen  and (max-width: 576px){
        .about-container{
            margin: 5rem 0;
        }
        .about-container .title h2{
            font-size: 1.5rem;
        }
        .about-container .title h1{
            font-size: 3rem;
        }
        .about-container .title{
            margin-bottom: 5rem;
        }
        .about-container .content-container{
            flex-direction: column-reverse;
            padding: 1rem 2rem;
        }
        .about-container .content-container .memoji{
            margin-top: 4rem;
        }
        .about-container .content-container .memoji img{
            width: 100%;
        }
        .about-container .content-container .memoji .social-links a{
            font-size: 3rem;
        }
        .about-container .content-container .content{
            width: 100%;
        }
        .about-container .content-container .content .about-me p{
            font-size: 1.3rem;
        }
        .about-container .content-container .content .about-me{
            margin-bottom: 2rem;
        }
        .about-container .content-container .content .links{
            background: transparent;
        }
        .about-container .content-container .content .links a{
            font-size: 1.3rem;
            font-weight: 600;
        }
    }
</style>