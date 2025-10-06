<script setup>
import Categories from './Categories.vue';
import Search from './Search.vue';
import Banner from './Banner.vue';
</script>

<template>
    <!-- Hero Section Begin -->
    <section class="hero">
        <div class="container">
            <div class="row">
                <div class="col-lg-3">
                    <Categories />
                </div>
                <div class="col-lg-9">
                    <Search />
                    <Banner />
                </div>
            </div>
        </div>
    </section>
    <!-- Hero Section End -->
</template>
