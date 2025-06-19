<script setup>
import lionLogo from '@/assets/img/lion-logo.svg'
import { useI18n } from 'vue-i18n'

const { t } = useI18n()
</script>

<template>
  <header class="header" :style="{
    backgroundImage: `url(${lionLogo})`,
    backgroundRepeat: 'no-repeat',
    backgroundPosition: 'right center',
    backgroundSize: '50%' 
  }">
    <img src="@/assets/img/lion-logo.svg" alt="lion logo" class="header__logo" />
    <div class="header__content">
      <div>
        <p class="slogan">{{ t('header-slogan') }}</p>
        <h1 class="header__content__heading">Polygone's</h1>
      </div>
      <div class="header__content__subheading">
        <span>{{ t('header-desc-1') }}</span>
        <span>{{ t('header-desc-2') }}</span>
      </div>
      <div class="btn">
        {{ t('header-btn') }}
      </div>
    </div>
  </header>
</template>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 2rem;
  background-color: #003787; 
  min-height: 250px;
  color: white;
  height: 100vh;
}
.header__logo {
  width: 100%;
  height: auto;
  display: none;
}
.slogan {
 color: var(--light-text-color, #FFF);
font-family: Montserrat;
font-size: 20px;
font-style: normal;
font-weight: 600;
line-height: normal;
}
.header__content {
    display: flex;
    flex-direction: column;
    gap: 1.6rem;
    max-width: 1200px;
    width: 100%;
  margin: 0 auto;
  padding: 0 1rem;
}
.header__content__heading {
  font-size: 9.6rem;
  font-weight: bold;
  margin: 0.5rem 0;
  font-family: 'Blogh', sans-serif;
  text-transform: uppercase;
}
.header__content__subheading {
  display: flex;
  flex-direction: column;
  font-size: 1.6rem;
  font-weight: 600;
  color: #fff;
}

.btn {
  background-color: #3781B0;
  display: inline-flex;
  color: #fff;
  padding: 15px 40px;
  border-radius: 5px;
  cursor: pointer;
  margin-top: 1rem;
  width: fit-content;
}
.btn:hover {
    background: #3c8cbe;
}
@media (max-width: 1280px) {
   .header {
    background-image: none !important;
    flex-direction: row-reverse;
    height: auto;
    padding: 0;
    
  }
   .header__logo {
    display: block;
    width: 400px;
  }
   .header__content{
  padding: 2.4rem;
  align-items: center;
 }
 .header__content__heading{
  font-size: 5rem;
 }
}
  
@media (max-width: 768px) {
 .header{
  flex-direction: column;
 }
 .header__logo {
    width: 100%;
  
  }

}
</style>
