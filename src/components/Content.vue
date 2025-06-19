<template>
    <section>
            <div class="content">
        <div class="content_description">
            <h2 class="heading-2">Polygone's</h2>
            <p>
                Née à Lyon pour donner une voix aux habitants et faire de chaque gone un acteur de sa ville !
            </p>
            <p>
                Elle propose une carte interactive, un fil d’actualité locale et un système de signalement en direct, permettant à chacun de participer activement à l’amélioration de son environnement quotidien.
            </p>
            <p>
                Portée par des valeurs d’inclusion, de transparence et de durabilité, elle accompagne la transformation des quartiers lyonnais en donnant à chacun les moyens d’agir.
polyGONE’S, c’est plusieurs gones, une même volonté : faire vivre la ville autrement.
            </p>
        </div>
        <div class="content_image">
            <img class="hex-img" src="@/assets/img/hex-2.png" alt="green" />
            <img class="hex-img offset" src="@/assets/img/hex-1.png" alt="green" />

        </div>
    </div>
    </section>

</template>
<style scoped>
section {
   padding: 4.8rem 0;
}
.content {
    display: flex;
    align-items: flex-start;
}

.content_description {
    display: flex;
    flex-direction: column;
    gap: 5rem;
    font-size: 1.6rem;
    line-height: 1.5;
    color: #737373;
}
.content-image{
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 4rem;
  padding: 2rem;
}

.hex-img {
  width: 250px;
  height: auto;
}

.offset {
  margin-left: 80px; 
}
</style>