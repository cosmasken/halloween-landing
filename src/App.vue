<script setup>
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

</style>
