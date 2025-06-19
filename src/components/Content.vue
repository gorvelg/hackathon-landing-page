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
            <div class="hex-img-hover">
                <img class="hex-img" src="@/assets/img/hex-2.png" alt="green" />
                <img class="poly" src="@/assets/img/poly-1.svg" alt="polygon">
            </div>
            <div class="hex-img-hover">
                <img class="hex-img offset" src="@/assets/img/hex-1.png" alt="green" />
                <img class="poly-2" src="@/assets/img/poly-2.svg" alt="polygon">
            </div>

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
.content_image{
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  gap: 4rem;
  padding: 2rem;
  width: 100%;
}
.hex-img-hover {
  position: relative;
  width: 250px;
  height: auto;
}

.hex-img {
  width: 100%;
  display: block;
  position: relative;
  z-index: 2;
}

.poly {
  width: 100%;
  position: absolute;
  top: 2px;
  left: 0;
  z-index: 1;
  transition: transform 0.3s ease;
}
.poly-2{
   width: 100%;
  position: absolute;
  top: 10px;
  left: 80px;
  z-index: 1;
  transition: transform 0.3s ease;
}


.hex-img-hover:hover .poly{
  transform: translate(12px, 12px);
}
.hex-img-hover:hover .poly-2 {
    transform: translate(12px, 24px);
}


.offset {
  margin-left: 80px; 
}
</style>