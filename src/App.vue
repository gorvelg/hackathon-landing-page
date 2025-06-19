<script setup>
import Header from '@/components/Header.vue';
import Content from '@/components/Content.vue';
import Features from '@/components/Features.vue';
import Testimonials from '@/components/Testimonials.vue';
import Numbers from '@/components/Numbers.vue';
</script>

<template>
  <Header />
  
  <div class="wrapper">
    <Content/>
    <Features />
  </div>
  <Testimonials />
  <div class="wrapper">
    <Numbers/>
  </div>
</template>

<style scoped>
.wrapper {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1rem;
}

@media (min-width: 600px) {
  .wrapper {
    padding: 0 2rem;
  }
}

@media (min-width: 1024px) {
  .wrapper {
    padding: 0 3rem;
  }
}
</style>
