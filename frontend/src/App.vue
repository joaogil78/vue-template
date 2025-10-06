<script setup>
import { onMounted } from 'vue';
import { RouterView } from 'vue-router';
import Humberger from '@/components/Humberger.vue';
import Header from '@/components/Header.vue';
import Hero from '@/components/Hero.vue';
import Footer from '@/components/Footer.vue';
import { preloader, setBg, humberger, navigation } from '@/assets/js/main.js';

onMounted(() => {
  preloader(),
  setBg(),
  humberger(),
  navigation();
});
</script>

<template>
  <!-- Page Preloder -->
  <div id="preloder">
      <div class="loader"></div>
  </div>

  <Humberger />
  <Header />
  <Hero />

  <RouterView />

  <Footer />
</template>
