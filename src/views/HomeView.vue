<script setup>
import { ref } from 'vue';
import Categori from '../components/homepage/Categori.vue';
import Hero from '../components/homepage/Hero.vue';

const categories = ref([
  {
    id: '1',
    path: '#',
    image: 'categories-1.jpg',
    text: 'Mobile UI Kit',
    desc: '731 items'
  }, {
    id: '2',
    path: '#',
    image: 'categories-2.jpg',
    text: 'Fonts',
    desc: '657 items'
  }, {
    id: '3',
    path: '#',
    image: 'categories-3.jpg',
    text: 'Icon Set',
    desc: '83,559 items'
  }, {
    id: '4',
    path: '#',
    image: 'categories-4.jpg',
    text: 'Website Ui Kit',
    desc: '4,500 items'
  }
])

const items = ref([
  {
    id: '1',
    path: '#',
    image: 'items-1.jpg',
    text: 'Mobile Ui Kit',
    desc: 'Mobile UI Kit'
  }, {
    id: '2',
    path: '#',
    image: 'items-2.jpg',
    text: 'Online Doctor Consultation',
    desc: 'Mobile UI Kit'
  }, {
    id: '3',
    path: '#',
    image: 'items-3.jpg',
    text: 'Banking Crypto',
    desc: 'Mobile UI Kit'
  }
])
</script>

<template>
  <main>
    <Hero />
    <Categori :datas="categories" title="Top Categories" />
    <Categori :datas="items" title="New Items" className="lg:w-1/3" />
  </main>
</template>
