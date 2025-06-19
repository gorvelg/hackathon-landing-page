<template>
    <section>
            <div class="content">
        <div class="content_description">
            <h2 class="heading-2">Polygone's</h2>
            <p>
                {{ $t('content-1') }}
            </p>
            <p>
               {{ $t('content-2') }}
            </p>
            <p>
               {{ $t('content-3') }}
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