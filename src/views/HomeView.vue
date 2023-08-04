<template>
  <div class="home">
    <Carou_sel class="carousel" v-slot="{ currentSlide }">
      <Carousel_Slide v-for="(slide, index) in carouselSlides" :key="index">
        <div class="slide-info" v-show="currentSlide === index + 1">
          <img :src="require(`../assets/${slide}.jpg`)" alt="" />
        </div>
      </Carousel_Slide>
    </Carou_sel>
  </div>
</template>

<script setup>
import Carou_sel from "@/components/Caru_sel.vue/Carou_sel.vue";
import Carousel_Slide from "@/components/Caru_sel.vue/Carousel_Slide.vue";
import { ref } from "vue";
const carouselSlides = ref(["img-1", "img-2", "img-3", "img-4"]);
</script>
<style lang="scss" scoped>
.home {
  width: 100%;
}

.carousel {
  position: relative;
  max-height: 100vh;
  height: 100vh;

  .slide-info {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    max-height: 100%;
    height: 100%;
  }

  img {
    min-width: 100%;
    height: 100%;
    object-fit: cover;
  }
}
</style>
