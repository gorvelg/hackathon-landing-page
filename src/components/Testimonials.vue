<template>
  <section>
    <div class="testimonials">
      <div class="overlay"></div>

      <div class="testimonials-content">
        <h2 class="testimonials-heading">Donnez votre avis !</h2>
        <div class="testimonial">
          <p>"Polygone's a transformé ma façon de voir mon quartier. Je me sens plus impliqué et écouté."</p>
          <span>- Camille, habitante de la Duchère</span>
        </div>
        <div class="btn">Lire les avis</div>
      </div>
    </div>
  </section>
</template>

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
  text-align: center;
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
}

</style>