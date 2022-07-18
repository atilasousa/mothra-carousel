<script setup lang="ts">
import AsCarousel from './components/AsCarousel.vue';
</script>

<template>
  <div class="wrapper">

    <as-carousel></as-carousel>
  </div>
</template>

<style lang="scss">
.wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
}

.red {
  border: 1px solid red !important;
}

.blue {
  border: 1px solid blue !important;
}
</style>
