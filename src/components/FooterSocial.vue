
<template>
  <div class="footer-column">
    <h4>Contact</h4>
    <p class="text">{{ $t('footer-subtitle-11') }}</p>
    <div class="icons">
      <img src="@/assets/icons/facebook.svg" alt="Facebook" />
      <img src="@/assets/icons/instagram.svg" alt="Instagram" />
      <img src="@/assets/icons/twitter.svg" alt="Twitter" />
    </div>
  </div>
</template>

<style scoped>
h4{
    font-weight: 700;
  margin-bottom: 1rem;
}
.text {
  color: gray;
  margin: 0.5rem 0 1rem;
}
.icons img {
  width: 24px;
  margin-right: 1rem;
  cursor: pointer;
}
</style>
