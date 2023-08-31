<script setup>
import tor1 from "../assets/tor1-img.png"
import tor2 from "../assets/tor2-img.png"
import tor3 from "../assets/tor3-img.png"
import tor4 from "../assets/tor4-img.png"
import tor5 from "../assets/tor5-img.png"
import tor6 from "../assets/tor-6-img.png"

const tots = [
  {
    title: 'Candy',
    image: tor1,
    desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id id consequat, eu faucibus nulla. Ultrices mattis lacus, sed maecenas nascetur.'
  },
  {
    title: 'Ghost',
    image: tor2,
    desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id id consequat, eu faucibus nulla. Ultrices mattis lacus, sed maecenas nascetur.'
  },
  {
    title: 'Grave',
    image: tor3,
    desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id id consequat, eu faucibus nulla. Ultrices mattis lacus, sed maecenas nascetur.'
  },
  {
    title: 'House',
    image: tor4,
    desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id id consequat, eu faucibus nulla. Ultrices mattis lacus, sed maecenas nascetur.'
  },
  {
    title: 'Spider',
    image: tor5,
    desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id id consequat, eu faucibus nulla. Ultrices mattis lacus, sed maecenas nascetur.'
  },
  {
    title: 'Bone',
    image: tor6,
    desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id id consequat, eu faucibus nulla. Ultrices mattis lacus, sed maecenas nascetur.'
  },
]

</script>

<template>
  <section id="trick-or-treat" class="flex flex-col items-center py-32">
    <h2 class="mt-10 mb-28 text-5xl md:text-6xl font-bold text-white">Trick Or Treat</h2>
    <div class="grid grid-cols-2 lg:grid-cols-3 gap-5 lg:gap-10">
      <div
          v-for="(tot, i) of tots"
          :key="tot.title"
          class="grid place-items-center text-center gap-5 p-8 rounded-md text-white bg-gradient-to-b from-primary-200/20 to-primary-200/10"
          :class="i === 1 && 'from-primary-200/50 to-primary-200/30 lg:-translate-y-10'
        "
      >
        <div>
          <img :src="tot.image" alt="">
        </div>
        <h3 class="text-2xl lg:text-4xl font-bold">{{ tot.title }}</h3>
        <p class="w-[90%] hidden md:block">{{ tot.desc }}</p>
      </div>
    </div>
  </section>
</template>