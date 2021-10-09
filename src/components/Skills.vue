<template>
    <!-- Skills Container Start  -->
    <div class="skills-container" id="skills">
        <div class="title">
            <h2>Skills</h2>
            <h1>What I know</h1>
        </div>
        <div class="content-container">
            <div class="content">
                <p>These are just some of the technologies & apps that I use to build my programs</p>
            </div>
            <div class="tools">
                <div class="tool">Html</div>
                <div class="tool">Css</div>
                <div class="tool">JavaScript</div>
                <div class="tool">Vue</div>
                <div class="tool">Gsap</div>
                <div class="tool">Particles.js</div>
            </div>
            <div class="tools">
                <div class="tool"><img src="../assets//adobe-xd.svg" alt="Adobe XD"></div>
                <div class="tool"><img src="../assets//vscode.svg" alt="Visual Studio Code"></div>
                <div class="tool"><img src="../assets//figma.svg" alt="Figma"></div>
            </div>
        </div>
    </div>
    <!-- Skills Container End  -->
</template>

<script>
    export default {
        name: 'Skills',
    }
</script>

<style scoped>
    .skills-container{
        position: relative;
        width: 100%;
        margin: 15rem 0;
    }
    .skills-container .title{
        width: 100%;
        position: relative;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-bottom: 10rem;
    }
    .skills-container .title h2{
        font-size: 3rem;
        color: var(--accent-1);
        text-transform: uppercase;
    }
    .skills-container .title h1{
        font-size: 5rem;
        color: var(--accent-2);
        text-transform: uppercase;
    }
    .skills-container .content{
        position: relative;
        width: 100%;
    }
    .skills-container .content p{
        font-size: 2rem;
        color: var(--font-light);
        text-align: center;
        margin-bottom: 2rem;
    }
    .skills-container .content-container .tools{
        width: 100%;
        padding: 3rem;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-wrap: wrap;
    }
    .skills-container .content-container .tools:nth-child(2) .tool{
        padding: 1rem 2rem;
        background: var(--accent-1);
        border-radius: 2rem;
        font-size: 2rem;
        color: var(--font-light);
        margin: 1rem;
    }
    .skills-container .tools .tool img{
        width: 10rem;
        height: 10rem;
        margin: 2rem;
    }
    @media screen and (max-width: 768px) {
        .skills-container{
            margin: 5rem 0;
        }
        .skills-container .title{
            margin-bottom: 5rem;
        }
        .skills-container .title h1{
            font-size: 3rem;
        }
        .skills-container h2{
            font-size: 1.5rem;
        }
        .skills-container .content{
            padding: 0 .5rem;
        }
        .skills-container .content p{
            font-size: 1.3rem;
        }
        .skills-container .content-container .tools:nth-child(2) .tool{
            font-size: 1.3rem;
        }
        .skills-container .tools .tool img{
            width: 5rem;
            height: 5rem;
        }
    }
    @media screen and (max-width: 576px) {
        .skills-container{
            margin: 5rem 0;
        }
        .skills-container .title{
            margin-bottom: 5rem;
        }
        .skills-container .title h1{
            font-size: 3rem;
        }
        .skills-container h2{
            font-size: 1.5rem;
        }
        .skills-container .content{
            padding: 0 .5rem;
        }
        .skills-container .content p{
            font-size: 1.3rem;
        }
        .skills-container .content-container .tools:nth-child(2) .tool{
            font-size: 1.3rem;
        }
        .skills-container .tools .tool img{
            width: 5rem;
            height: 5rem;
        }
    }
</style>