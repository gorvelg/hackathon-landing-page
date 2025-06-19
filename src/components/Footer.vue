<script setup>
import FooterColumn from './FooterColumn.vue'
import FooterSocial from './FooterSocial.vue'
import { useI18n } from 'vue-i18n'

const { t } = useI18n()
</script>

<template>
  <footer class="footer">
    <FooterSocial />
    <FooterColumn
      title="Informations"
      :items="[
        t('footer-subtitle-21'),
        'IUT Troyes',
        'IUT Castres'
      ]"
    />
    <FooterColumn
      :title="t('footer-title-3')"
      :items="[
        t('footer-subtitle-31'),
        t('footer-subtitle-32'),
        t('footer-subtitle-33'),
        'Cookies'
      ]"
    />
  </footer>
</template>


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
