<script setup>
import Navbar from './components/Navbar.vue';
import Hero from './components/Hero.vue';
import CTA from './components/CTA.vue';
import Shorten from './components/Shorten.vue';
import Footer from './components/Footer.vue';
</script>

<template>
  <Navbar></Navbar>
  <Hero></Hero>
  <Shorten
  :links="[
    {
      original: 'https://frontendmentor.io',
      short: 'https://rel.ink/k3lKyk',
      isFocus: false
    },
    {
      original: 'https://twitter.com/fontendmentor',
      short: 'https://rel.ink/gxOXp9',
      isFocus: true
    },
    {
      original: 'https://linkedin.com/frontend-mentor',
      short: 'https://rel.ink/gob3X9',
      isFocus: false
    }
  ]"
  ></Shorten>
  <CTA></CTA>
  <Footer></Footer>
</template>

<style scoped>

</style>
