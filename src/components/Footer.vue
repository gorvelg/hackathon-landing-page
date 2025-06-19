<template>
  <footer class="footer">
    <FooterSocial />
    <FooterColumn title="Informations" :items="['À propos', 'IUT Troyes', 'IUT Castres']" />
    <FooterColumn title="Ressources" :items="['Confidentialité', 'Conditions d\'utilisation', 'Mentions légales', 'Cookies']" />
  </footer>
</template>

<script setup>
import FooterColumn from './FooterColumn.vue'
import FooterSocial from './FooterSocial.vue'
</script>

<style scoped>
.footer {
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  padding: 4rem;
  background-color: #fff;
  color: #000;
  gap: 2rem;
}
</style>
