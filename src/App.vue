<template>
  <PreLoader />
  <Hero />
  <About />
  <Skills />
  <Services />
  <Portfolio />
  <Contact />
  <ToTop />
</template>

<script>

import PreLoader from './components/PreLoader.vue'
import Hero from './components/Hero.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue'
import Services from './components/Services.vue'
import Portfolio from './components/Portfolio.vue'
import Contact from './components/Contact.vue'
import ToTop from './components/ToTop.vue'

export default {
  name: 'App',
  components: {
    Hero,
    About,
    PreLoader,
    Services,
    Portfolio,
    ToTop,
    Skills,
    Contact,
  },
}
</script>

<style>
:root{
  --bg-dark: #11112d;
  --bg-light: #DEDEEA;
  --font-light: #FFFFFF;
  --font-dark: #11112D;
  --accent-1: #30BCED;
  --accent-1-50: #01F0FF;
  --accent-2: #F46E0C;
  --accent-2-50: #F68634;
}
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
html{
  font-size: 62.5%;
  font-family: 'Poppins', sans-serif;
  scroll-behavior: smooth;
}
body{
  background: var(--bg-dark);
  overflow-y: auto;
}
body::-webkit-scrollbar {
  width: 1rem;
}
 
body::-webkit-scrollbar-track {
  background: var(--accent-1);
  border-radius: 3rem;
}
 
body::-webkit-scrollbar-thumb {
  background-color: var(--accent-2);
  border-radius: 3rem;
}
body.no-scroll{
  overflow-y: hidden;
}
</style>
