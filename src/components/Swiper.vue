<script setup>
// import Swiper core and required modules
import { Pagination } from 'swiper';

// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';
import 'swiper/css/pagination';

const modules = [Pagination]

</script>

<template>
  <swiper
      :modules="modules"
      :slides-per-view="1"
      :pagination="{ clickable: true }"
      class="pb-8"
  >
    <swiper-slide class="grid place-items-center">
        <img src="../assets/home1-img.png" class="w-2/3 lg:w-[90%]" alt="Slide image 1" />
    </swiper-slide>
    <swiper-slide class="grid place-items-center">
      <img src="../assets/slider_img1.png" class="w-2/3 lg:w-[90%]" alt="Slide image 2"/>
    </swiper-slide>
    <swiper-slide class="grid place-items-center">
      <img src="../assets/slider_img2.png" class="w-2/3 lg:w-[90%]" alt="Slide image 3" />
    </swiper-slide>
    <swiper-slide class="grid place-items-center">
      <img src="../assets/slider_img3.png" class="w-2/3 lg:w-[90%] " alt="Slide image 4" />
    </swiper-slide>
    <swiper-slide class="grid place-items-center h-60">
      <img src="../assets/slider_img4.png" class="w-[90%]" />
    </swiper-slide>
  </swiper>
</template>

<style>

</style>