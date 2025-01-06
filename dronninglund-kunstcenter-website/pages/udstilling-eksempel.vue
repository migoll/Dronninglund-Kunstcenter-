<template>
<main>
  <section>
    <div class="udstilling-landing-page">
  <p>23343  -  34342</p>
  <h1>hej</h1>
  <img src="/images/dk-sllide7.jpg" alt="">
    </div>
  </section>
  <section>
    <div class="udstilling-information">
    <h2>Foreningen Danske Kunsthåndværkere & Designere</h2>
    <p>Udstillingen laves i samarbejde med “Danske Kunsthåndværkere & Designere (DKoD)”, der er en forening for professionelle kunsthåndværkere og designere. Foreningen blev stiftet i 1976 og har ca. 500 medlemmer. Foreningen arbejder for en kunstnerisk og håndværksmæssig udvikling af dansk kunsthåndværk og design og for medlemmernes faglige og erhvervsmæssige interesser, samt at udbrede kendskabet til og brugen af kunsthåndværkere/designere og deres arbejder i alle dele af samfundet.
  Udstillingen er støttet af Statens Kunstfond</p>
  <div class="medvirkende">
    <div class="medvirkende-header" @click="toggle">
      <h3>Medvirkende</h3>
      <img v-if="!isOpen" src="/icons/plus-solid.svg" alt="Plus icon">
      <img v-if="isOpen" src="/icons/minus-solid.svg" alt="Minus icon">
    </div>
    <div class="medvirkende-navne" :class="{ open: isOpen }">
      <p>Anne Jensen</p>
      <p>Anne Jensen</p>
      <p>Anne Jensen</p>
      <p>Anne Jensen</p>
      <p>Anne Jensen</p>
    </div>
  </div>
    </div>
  </section>
  <section>
    <div class="image-gallery-udstilling">
      <img src="/images/dk-sllide7.jpg" alt="">
      <img src="/images/dk-sllide7.jpg" alt="">
      <img src="/images/dk-sllide7.jpg" alt="">
      <img src="/images/dk-sllide7.jpg" alt="">
      <img src="/images/dk-sllide7.jpg" alt="">
      <img src="/images/dk-sllide7.jpg" alt="">
      <img src="/images/dk-sllide7.jpg" alt="">
    </div>
  </section>
</main>
</template>
<script>
    export default {
  data() {
    return {
      isOpen: false
    };
  },
  methods: {
    toggle() {
      this.isOpen = !this.isOpen;
    }
  }
};
</script>
<style scoped>
    .udstilling-landing-page {
    background: #000000;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    padding-top: 5rem;
    padding-bottom: 5rem;
  }

  .udstilling-landing-page p {
    color: rgba(255, 255, 255, 0.50);
    border: 2px solid rgba(255, 255, 255, 0.20);
    border-radius: 5px;
    padding: 15px 15px;
    font-size: 1rem;
  }

  .udstilling-landing-page h1 {
    color: white;
    padding-bottom: 3rem;
    font-size: 2rem;
    margin: 3rem 120px;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  .udstilling-landing-page img {
    width: 100%;
    max-width: 300px;
    margin: 0 20px;
  }

  .udstilling-information {
    margin: 3rem 20px;
    line-height: 1.5;
  }

  .udstilling-information h2 {
    font-size: 1.75rem;
  }

  .udstilling-information p {
    font-size: 1rem;
  }

  .medvirkende {
  background: #D9D9D9;
  margin-top: 2rem;
  margin-bottom: 5rem;
  border-radius: 15px;
  overflow: hidden;
}

.medvirkende h3 {
    font-size: 1.25rem;
}

.medvirkende img {
    width: 20px;
}

.medvirkende-header {
  background-color: #D9D9D9;
  padding: 10px;
  cursor: pointer;
  display: flex;
  justify-content: space-between;
  padding: 0 20px;
}

.medvirkende-navne {
  padding-left: 20px;
  padding-right: 20px;
  background-color: #f1f1f1;
  max-height: 0;
  overflow: hidden;
  transition: max-height 0.5s ease-out;
}

.medvirkende-navne.open {
  max-height: 500px;
}

.medvirkende-navne.open p {
    font-size: 1rem;
}
  
  .image-gallery-udstilling {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  justify-items: center;
  align-items: center;
  padding: 3rem 20px;
  background: #000000;
  gap: 3rem;
}

.image-gallery-udstilling img {
  max-width: 250px;
  width: 100%;
}

/* Add this new rule to center images that are alone in a row */
.image-gallery-udstilling img:last-child:nth-child(odd) {
  grid-column: 1 / -1;
}

</style>