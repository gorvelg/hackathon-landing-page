<script setup>
import Header from '@/components/Header.vue';
import Content from '@/components/Content.vue';
import Features from '@/components/Features.vue';
import Testimonials from '@/components/Testimonials.vue';
import Numbers from '@/components/Numbers.vue';
import Footer from '@/components/Footer.vue';
import { useI18n } from 'vue-i18n'

const { locale } = useI18n()
</script>

<template>
  <!-- Lang toggle -->
  <div class="lang-toggle">
    <button
      :class="{ active: locale === 'fr' }"
      @click="locale = 'fr'"
      aria-label="Passer au français"
    >
      🇫🇷
    </button>
    <button
      :class="{ active: locale === 'en' }"
      @click="locale = 'en'"
      aria-label="Switch to English"
    >
      🇬🇧
    </button>
  </div>

  <Header />
  <div class="wrapper">
    <Content />
    <Features />
  </div>
  <Testimonials />
  <div class="wrapper">
    <Numbers />
    <Footer />
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
.lang-toggle {
  position: fixed;
  top: 1rem;
  right: 1rem;
  z-index: 1000;
  background: white;
  border-radius: 8px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.15);
  display: flex;
  overflow: hidden;
}

.lang-toggle button {
  all: unset;
  cursor: pointer;
  font-size: 1.5rem;
  padding: 0.6rem 0.8rem;
  transition: background 0.2s ease;
}

.lang-toggle button:hover {
  background: #f0f0f0;
}

.lang-toggle button.active {
  background: #003787;
  color: white;
}
</style>
