<template>
  <section>   
    <div class="numbers-container">
      <div class="numbers-heading">
        <h2>Polygone's</h2>
        <span class="subtitle">{{ t('numbers-title') }}</span>
      </div>

      <div class="numbers">
        <div class="number-item">
          <h3>-20%</h3>
          <p>{{ t('numbers-1') }}</p>
        </div>
        <div class="number-item">
          <h3>2000</h3>
          <p>{{ t('numbers-2') }}</p>
        </div>
        <div class="number-item">
          <h3>4.5</h3>
          <div>
            <img src="@/assets/img/icn bxs-star-full.svg" alt="TrustPilot" >
            <img src="@/assets/img/icn bxs-star-full.svg" alt="TrustPilot" >
            <img src="@/assets/img/icn bxs-star-full.svg" alt="TrustPilot" >
            <img src="@/assets/img/icn bxs-star.svg" alt="TrustPilot" >
            <img src="@/assets/img/icn bx-star.svg" alt="TrustPilot" >
          </div>
          <p>{{ t('numbers-3') }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { useI18n } from 'vue-i18n'
const { t } = useI18n()
</script>

<style scoped>
.numbers-container {
    display: flex;
    padding: 4.8rem 0;
    gap: 2.4rem;
}
.numbers-heading {
    font-size: 5rem;
    font-weight: bold;
    text-align: center;
    color: #003787;
    font-family: 'Blogh', sans-serif; 
    text-transform: uppercase;
    letter-spacing: 2px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    
 
}
.subtitle {
    color: var(--text-color, #252B42);
font-family: Montserrat;
font-size: 24px;
font-style: normal;
font-weight: 600;
line-height: normal;
text-transform: lowercase;
margin: -32px 0;
}
.numbers {
    display: flex;
    justify-content: space-around;
    width: 100%;
    max-width: 1200px;
    margin-top: 2rem;
}
.number-item {
    text-align: center;
    flex: 1;    
    margin: 0 1rem;
}
.number-item h3 {
    color: #252B42;
text-align: center;
font-family: Montserrat;
font-size: 40px;
font-style: normal;
font-weight: 600;
line-height: normal;
}
.number-item p {
    font-size: 1.5rem;
    color: #333;
}
@media (max-width: 768px) {
 
  .numbers-container {
    flex-direction: column;
    align-items: center;
  }
  .numbers-heading {
    align-items: center;
    
  }
  .numbers-heading h2{
    font-size: 5rem;
  }
  .subtitle {
    margin: -16px 0;
  }
}
</style>