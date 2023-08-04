<template>
  <div class="carousel">
    <slot :currentSlide="currentSlide" />
    <div class="navigation">
      <div class="toggle left">
        <i class="fas fa-chevron-left"></i>
      </div>
      <div class="toggle right">
        <i class="fas fa-chevron-right"></i>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const currentSlide = ref(1);
</script>

<style lang="scss">
.navigation {
  padding: 0 16px;
  height: 100%;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
