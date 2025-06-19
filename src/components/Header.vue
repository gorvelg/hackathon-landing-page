<script setup>
import lionLogo from '@/assets/img/lion-logo.svg';
</script>

<template>
  <header class="header" :style="{
    backgroundImage: `url(${lionLogo})`,
    backgroundRepeat: 'no-repeat',
    backgroundPosition: 'right center',
    backgroundSize: 'auto 80%' 
  }">
    <div class="header__content">
      <p>Soyez tous connectés</p>
      <h1 class="header__content__heading">Polygone's</h1>
      <span>Application citoyenne</span>
      <span>Quartier de la Duchère - Lyon</span>
      <div class="btn">
        Télécharger l'application
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
}
.header__content {
    display: flex;
    flex-direction: column;
}
.header__content__heading {
  font-size: 9.6rem;
  font-weight: bold;
  margin: 0.5rem 0;
  font-family: 'Blogh', sans-serif;
  text-transform: uppercase;
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
</style>
