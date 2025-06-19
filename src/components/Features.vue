<script setup>
import FeatureCard from '@/components/FeatureCard.vue';
</script>
<template>
    <section>
            <h2 class="heading-2">Nos valeurs</h2>
    <div class="features">
        <FeatureCard
            name="Mobilité"
            description="Encourage une ville fluide et accessible, où chacun peut se déplacer facilement, durablement et en toute sécurité."
        />
        <FeatureCard
            name="Intégrité"
            description="La transparence est au cœur de son 
fonctionnement. polyGONE’S repose sur une
 information fiable, des échanges respectueux et 
une démarche honnête !"
        />
        <FeatureCard
            name="Respect"
            description="Elle défend un rapport harmonieux à la ville,
à ses habitants et à son environnement. 
Respect des différences, de l’espace public, 
du vivant : chaque action compte pour construire 
un cadre de vie partagé."
        />
        <FeatureCard
            name="Bien-être"
            description="polyGONE’S place le bien-être au centre de 
son engagement. Mieux vivre son quartier, 
c’est se sentir écouté, en sécurité, entouré, 
et fier de contribuer à une ville plus humaine."
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