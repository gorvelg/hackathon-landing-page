<template>
  <section>
    <div class="testimonials">
      <div class="overlay"></div>

      <div class="testimonials-content">
        <h2 class="testimonials-heading">{{ t('testimonials-title') }}</h2>
        <div class="testimonial">
          <p>{{ t('testimonials-subtitle') }}</p>
          <span>{{ t('testimonials-author') }}</span>
        </div>
        <div class="btn">{{ t('testimonials-button') }}</div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { useI18n } from 'vue-i18n'
const { t } = useI18n()
</script>


<style scoped>

.testimonials-heading {
    font-size: 40px;
    font-style: normal;
    font-weight: 700;
    line-height: 50px;
    letter-spacing: 2px;
}

.testimonials {
  position: relative;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  font-family: Montserrat;
  color: #fff;
  background: url('../assets/img/ecoquartiers.jpg') no-repeat center center;
  background-size: cover;
  /* background-attachment: fixed;  */
  padding: 4.8rem 0;
  overflow: hidden;
  height: 430px;
}


.overlay {
  position: absolute;
  inset: 0;
  background-color: #003787;
  opacity: 0.7;
  z-index: 1;
}

.testimonials-content {
    display: flex;
    align-items: center;
    flex-direction: column;
    gap: 1.6rem;
    margin-bottom: 2rem;
    position: relative;
    z-index: 2; 
}

.btn {
  display: flex;
  padding: 15px 36px;
  flex-direction: column;
  align-items: center;
  gap: 10px;
  border-radius: 37px;
  border: 1px solid #FAFAFA;
  position: relative;
  z-index: 2;
  width: fit-content;
  transition: 25ms transform ease-in;
  cursor: pointer;
}
.btn:hover {
    transform: scale(1.05);
}

@media (max-width: 768px) {
  

  
  
 
 
}

</style>