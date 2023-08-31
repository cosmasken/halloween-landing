<script setup>
import HelloWorld from './components/HelloWorld.vue'
import Navbar from "./components/Navbar.vue";
import Hero from "./components/Hero.vue"
import Footer from "./components/Footer.vue"
import Category from "./components/Category.vue";
import TrickOrTreat from "./components/TrickOrTreat.vue";
import Subscribe from "./components/Subscribe.vue";
</script>

<template>
  <div class=" center p-16px sm:p-32 lg:p-64 overflow-x-hidden">
<Navbar/>
    <Hero/>
    <Category/>
    <TrickOrTreat/>
    <Subscribe/>
    <Footer/>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
