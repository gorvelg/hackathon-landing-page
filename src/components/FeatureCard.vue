<script setup>
const props = defineProps({
    name: {
        type: String,
        required: true
    },
    description: {
        type: String,
        required: true
    }
});
</script>
<template>
    <div class="feature-card">
        <h3 class="heading-3">{{ name }}</h3>
        <p class="feature-desc">{{ description }}</p>
    </div>
</template>
<style scoped>
.feature-card {
    display: flex;
    gap: 1.6rem;
    flex-direction: column;

}
.heading-3 {
    font-size: 5rem;
    font-weight: bold;
    margin-bottom: 10px;
    color: #3781B0;
    font-family: 'Blogh', sans-serif;
    text-transform: uppercase;
    letter-spacing: 2px;
}
.feature-desc {
    font-size: 1.6rem;
    color: #737373;
    line-height: 1.5;
}
@media (max-width: 768px) {
  

  .feature-card{
    align-items: center;
  }
  
}
</style>