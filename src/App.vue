<script setup>
import Header from '@/components/Header.vue';
import Content from '@/components/Content.vue';
import Features from '@/components/Features.vue';
</script>

<template>
  <Header />
  
  <main>
    <Content/>
    <Features />
  </main>
</template>

<style scoped>
main {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1rem;
}

@media (min-width: 600px) {
  main {
    padding: 0 2rem;
  }
}

@media (min-width: 1024px) {
  main {
    padding: 0 3rem;
  }
}
</style>
