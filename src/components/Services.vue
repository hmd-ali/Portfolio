<template>
    <!-- Services Container Start  -->
    <div class="services-container" id="services">
        <div class="title">
            <h2>services</h2>
            <h1>what i do</h1>
        </div>
        <div class="content-container">
            <!-- Cards Start -->
            <div class="cards">
                <!-- Card Start -->
                <div class="card">
                    <div class="icon">
                        <i class="fas fa-mobile"></i>
                    </div>
                    <h1>Responsive Design</h1>
                    <p>Designs optimized for Desktops, tablets and phones screens</p>
                </div>
                <!-- Card End  -->
                <!-- Card Start -->
                <div class="card">
                    <div class="icon">
                        <i class="fas fa-laptop-code"></i>
                    </div>
                    <h1>Web Design</h1>
                    <p>Designs updated with the latest trends</p>
                </div>
                <!-- Card End  -->
                <!-- Card Start -->
                <div class="card">
                    <div class="icon">
                        <i class="fas fa-palette"></i>
                    </div>
                    <h1>Graphic Design</h1>
                    <p>Hand crafted logos</p>
                </div>
                <!-- Card End  -->
                <!-- Card Start -->
                <div class="card">
                    <div class="icon">
                        <i class="fas fa-terminal"></i>
                    </div>
                    <h1>Clean Code</h1>
                    <p>Easy to read code with minimal errors</p>
                </div>
                <!-- Card End  -->
            </div>
            <!-- Cards End  -->
        </div>
    </div>
    <!-- Services Container End  -->
</template>

<script>
    export default {
        name: 'Services',
    }
</script>

<style scoped>
    .services-container{
        position: relative;
        width: 100%;
        margin: 15rem 0;
    }
    .services-container .title{
        width: 100%;
        position: relative;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-bottom: 10rem;
    }
    .services-container .title h2{
        font-size: 3rem;
        color: var(--accent-1);
        text-transform: uppercase;
    }
    .services-container .title h1{
        font-size: 5rem;
        color: var(--accent-2);
        text-transform: uppercase;
    }
    .services-container .cards{
        width: 100%;
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-wrap: wrap;
    }
    .services-container .cards .card{
        position: relative;
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        align-items: center;
        width: 50rem;
        height: 40rem;
        border-top: 2px solid var(--accent-2);
        border-left: 2px solid var(--accent-2);
        border-bottom: 2px solid var(--accent-1);
        border-right: 2px solid var(--accent-1);
        margin: 2rem;
        padding: 2rem;
        border-radius: 1.5rem;
        text-align: center;
    }
    .services-container .cards .card .icon{
        position: relative;
        width: 10rem;
        height: 10rem;
        background: var(--accent-2);
        border-radius: 50%;
        padding: 2rem;
        display: flex;
        align-items: center;
        justify-content: center;
        transition: all 300ms ease;
    }
    .services-container .cards .card:hover .icon{
        transform: scale(.9);        
    }
    .services-container .cards .card .icon i{
        font-size: 4rem;
        color: var(--font-light);
    }
    .services-container .cards .card h1{
        font-size: 3rem;
        color: var(--font-light);
    }
    .services-container .cards .card p{
        color: var(--font-light);
        font-size: 2rem;
    }
    @media screen and (max-width: 768px) {
        .services-container{
            margin: 5rem 0;
        }
        .services-container .title{
            margin-bottom: 5rem;
        }
        .services-container .title h1{
            font-size: 3rem;
        }
        .services-container .title h2{
            font-size: 1.5rem;
        }
    }
    @media screen and (max-width: 576px) {
        .services-container{
            margin: 5rem 0;
        }
        .services-container .title{
            margin-bottom: 5rem;
        }
        .services-container .title h1{
            font-size: 3rem;
        }
        .services-container .title h2{
            font-size: 1.5rem;
        }
    }
</style>