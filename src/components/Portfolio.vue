<template>
    <!-- Portfolio Container Start  -->
    <div class="portfolio-container" id="portfolio">
        <div class="title">
            <h2>Portfolio</h2>
            <h1>Latest Works</h1>
        </div>
        <div class="projects">
            <div class="project">
                <div class="image">
                    <img src="../assets/project-1.jpg" alt="Shabeb Website">
                </div>
                <div class="name">
                    <h1>Shabeb's Website</h1>
                    <div class="link">
                        <a title="Shabeb's Website" target="_blank" href="https://shabeb.netlify.app/"><span><i class="fas fa-link"></i>View Website</span></a>
                    </div>
                </div>
            </div>
            <div class="project">
                <div class="image">
                    <img src="../assets/project-2.jpg" alt="Weather App">
                </div>
                <div class="name">
                    <h1>Weather App</h1>
                    <div class="link">
                        <a title="Weather App" target="_blank" href="https://app-weather-ali.netlify.app/"><span><i class="fas fa-link"></i>Visit Website</span></a>
                    </div>
                </div>  
            </div>
            <div class="project">
                <div class="image">
                    <img src="../assets/project-3.jpg" alt="Rock Paper Scissors">
                </div>
                <div class="name">
                    <h1>Rock Paper Scissors</h1>
                    <div class="link">
                        <a title="Rock Paper Scissors Game" target="_blank" href="https://suspicious-mcclintock-5148a9.netlify.app/"><span><i class="fas fa-link"></i>Visit Website</span></a>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- Portfolio Container End  -->
</template>

<script>
    export default {
        name: 'Portfolio',
    }
</script>

<style scoped>
    .portfolio-container{
        position: relative;
        width: 100%;
        margin: 15rem 0;
    }
    .portfolio-container .title{
        width: 100%;
        position: relative;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-bottom: 10rem;
    }
    .portfolio-container .title h2{
        font-size: 3rem;
        color: var(--accent-1);
        text-transform: uppercase;
    }
    .portfolio-container .title h1{
        font-size: 5rem;
        color: var(--accent-2);
        text-transform: uppercase;
    }
    .portfolio-container .projects{
        width: 100%;
        padding: 5rem;
        position: relative;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
    }
    .portfolio-container .projects .project{
        position: relative;
        width: 50rem;
        height: 40rem;
        background: var(--bg-dark);
        border-radius: 2rem;
        border-top: 2px solid var(--accent-2);
        border-left: 2px solid var(--accent-2);
        border-right: 2px solid var(--accent-1);
        border-bottom: 2px solid var(--accent-1);
        margin: 2rem;
        padding: 2rem;
        display: flex;
        flex-direction: column;
    }
    .portfolio-container .projects .project .image{
        position: relative;
        width: 100%;
        transition: transform 500ms;
        overflow: hidden;
        border-radius: 1rem;
    }
    .portfolio-container .projects .project .image img{
        width: 100%;
        border-radius: 1rem;
        object-position: center;
        transition: transform 500ms;
        object-fit: cover;
    }
    .portfolio-container .projects .project .name{
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .portfolio-container .projects .project .name h1{
        font-size: 2rem;
        margin-top: 1rem;
        color: var(--font-light);
        font-weight: 300;
    }
    .portfolio-container .projects .project:hover .image img{
        transform: scale(1.1);
    }
    .portfolio-container .projects .project .link a{
        position: relative;
        text-decoration: none;
        color: var(--accent-1);
        font-size: 1.5rem;
    }
    .portfolio-container .projects .project .link a span i{
        margin-right: 1rem;
    }
    .portfolio-container .projects .project .link a::before{
        content: '';
        position: absolute;
        bottom: -.5rem;
        width: 0;
        height: 1px;
        background: var(--accent-1);
        transition: width 500ms;
    }
    .portfolio-container .projects .project .link a:hover::before{
        width: 100%;
    }
    @media screen and (max-width: 768px) {
        .portfolio-container{
            margin: 5rem 0;
        }
        .portfolio-container .title{
            margin-bottom: 5rem;
        }
        .portfolio-container .title h1{
            font-size: 3rem;
        }
        .portfolio-container .title h2{
            font-size: 1.5rem;
        }
        .portfolio-container .projects .project{
            height: 30rem;
            width: 100%;
        }
        .portfolio-container .projects{
            padding: 2rem;
        }
    }
    @media screen and (max-width: 576px) {
        .portfolio-container{
            margin: 5rem 0;
        }
        .portfolio-container .title{
            margin-bottom: 5rem;
        }
        .portfolio-container .title h1{
            font-size: 3rem;
        }
        .portfolio-container .title h2{
            font-size: 1.5rem;
        }
        .portfolio-container .projects .project{
            height: 30rem;
            width: 100%;
        }
        .portfolio-container .projects{
            padding: 2rem;
        }
        .portfolio-container .projects .project .name{
            flex-direction: column;
        }
    }
</style>