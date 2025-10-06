<script setup>
import CategoriesSlider from '@/components/CategoriesSlider.vue';
import Featured from '@/components/Featured.vue';
import Banners from '@/components/Banners.vue';
import LatestProducts from '@/components/LatestProducts.vue';
import BlogPosts from '@/components/BlogPosts.vue';
import { onMounted } from 'vue';
import {
  categoriesSlider,
  latestProductsSlider,
  productsDiscontSlider,
  productDetailsSlider,
  niceSelect,
  singleProducts,
} from '@/assets/js/main.js';

onMounted(() => {
  categoriesSlider(),
  latestProductsSlider(),
  productsDiscontSlider(),
  productDetailsSlider(),
  niceSelect(),
  singleProducts();
});
</script>

<template>

  <CategoriesSlider />
  <Featured />
  <Banners />
  <LatestProducts />
  <BlogPosts />

</template>
