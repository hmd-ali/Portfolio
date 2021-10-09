<template>
    <!-- ToTop Start  -->
    <div :class="['to-top' , !isScrolled ? 'hide' : '']">
        <a href="#hero"><span><i class="fas fa-chevron-up"></i></span></a>
        <span>Back to top</span>
    </div>
    <!-- ToTop End  -->
</template>

<script>
    export default {
        name: 'ToTop',
        data(){
            return{
                isScrolled: false
            }
        },
        mounted(){
            window.addEventListener('scroll' , () => {
                window.scrollY > 0 ? this.isScrolled = true : this.isScrolled = false
            })
        }
    }
</script>

<style scoped>
    .to-top{
        position: fixed;
        bottom: 2%;
        right: 2%;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        transition: 300ms opacity .5s ease;
        opacity: 1;
    }
    .to-top > span{
        color: var(--accent-1);
        font-size: 1.4rem;
    }
    .to-top.hide{
        display: none;
        opacity: 0;
    }
    .to-top a{
        text-decoration: none;
        color: var(--accent-2);
        font-size: 4rem;
    }
</style>