<script setup>
import FeatureCard from '@/components/FeatureCard.vue';
</script>
<template>
    <section>
            <h2 class="heading-2">{{ $t('feature-heading') }}</h2>
    <div class="features">
      <FeatureCard
  :name="$t('feature-1-title')"
  :description="$t('feature-1')"
/>

<FeatureCard
  :name="$t('feature-2-title')"
  :description="$t('feature-2')"
/>

<FeatureCard
  :name="$t('feature-3-title')"
  :description="$t('feature-3')"
/>

<FeatureCard
  :name="$t('feature-4-title')"
  :description="$t('feature-4')"
/>

    </div>
    </section>

</template>
<style scoped>
section {
    padding: 4.8rem 0;
}
.features {
    display: grid;
    grid-template-columns: repeat(2, minmax(300px, 1fr));
    gap: 2rem;
    justify-content: center;
}
</style>