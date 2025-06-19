
<template>
  <div class="footer-column">
    <h4>{{ title }}</h4>
    <ul>
      <li v-for="(item, index) in items" :key="index">{{ item }}</li>
    </ul>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  items: Array
});
</script>

<style scoped>
.footer-column h4 {
  font-weight: 700;
  margin-bottom: 1rem;
}
.footer-column li {
  color: gray;
  margin-bottom: 0.5rem;
  list-style: none;
}
</style>
