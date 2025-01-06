<template>
  <section class="åbningstider center-section">
    <h1>Praktisk information</h1>
    <h2>Åbningstider</h2>
    <div class="åbningsdage-line">
      <p>Mandag - Fredag</p>
      <p>13:00 - 17:00</p>
    </div>
    <div class="åbningsdage-line">
      <p>Lørdag - Søndag</p>
      <p>11:00 - 17:00</p>
    </div>
    <div class="divider-hr"></div>
    <div class="åbningsdage-line">
      <p>Åbent hele påsken</p>
      <p>11:00 - 17:00</p>
    </div>
    <div class="divider-hr"></div>
    <div class="åbningsdage-line">
      <p>Skærstorsdag - 2. påskedag</p>
      <p>11:00 - 17:00</p>
    </div>
    <div class="divider-hr"></div>
    <div class="åbningsdage-line">
      <p>Kr. Himmelfartsdag + 2. pinsedag</p>
      <p>11:00 - 17:00</p>
    </div>
  </section>
  <section class="center-section">
    <h2>Handicapforhold</h2>
    <p>
      Alle handicappede er meget velkomne på Dronninglund Kunstcenter.Vi har
      netop til 2024 sæsonen, fået installeret elevator og handicap toilet, så
      det er nu muligt for gangbesværede at besøge alle 3 plan.
    </p>
    <p>
      OBS Handicappede betaler fuld pris, men evt. hjælper kommer gratis ind.
    </p>
  </section>
  <section class="center-section">
    <h2>Offentlig transport og parkering</h2>
    <p>Vi tilbyder egen parkeringsplads.</p>
    <p>
      Hvis du vil benytte dig af offentlig transport går der bus i nærheden,
      hvor du kan slutte af med en kort gåtur til Kunstcenteret.
    </p>
    <button class="reverse-button-black">Se busplan</button>
  </section>
  <section class="center-section accordion-section">
    <div class="accordion">
      <div class="accordion-header" @click="toggleAccordion">
        <h3>Bestyrelsen</h3>
        <button class="accordion-toggle">
          {{ isAccordionOpen ? "▲" : "▼" }}
        </button>
      </div>
      <div class="accordion-content" v-show="isAccordionOpen">
        <ul>
          <li>
            <strong>Christian Christensen</strong> - Formand<br />Tlf: 40316891
          </li>
          <li>
            <strong>Elly Ørnberg</strong> - Næstformand<br />Tlf: 21761628
          </li>
          <li><strong>Karen Axen</strong> - Kasserer<br />Tlf: 22993844</li>
          <li><strong>Karin Sanden</strong> - Sekretær<br />Tlf: 28771488</li>
          <li><strong>Jørgen Abildgaard</strong><br />Tlf: 21286372</li>
          <li><strong>Birgit Bang Henriksen</strong> - Suppleant</li>
        </ul>
        <a href="#" class="accordion-link">Vedtægter</a>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";

const isAccordionOpen = ref(false);

const toggleAccordion = () => {
  isAccordionOpen.value = !isAccordionOpen.value;
};
</script>

<style scoped>
.accordion-section {
  margin-top: 2rem;
  max-width: 1080px;
  padding-block: 2rem;
  margin: 0 auto;
}

.accordion {
  border: 3px solid black;
  border-radius: 6px;
  overflow: hidden;
  max-width: 1;
}

.accordion-header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: black;
  color: white;
  padding: 0.5rem 1rem;
  cursor: pointer;
}

.accordion-toggle {
  background: none;
  border: none;
  color: white;
  font-size: 16px;
  cursor: pointer;
}

.accordion-content {
  padding: 1rem;
  background-color: white;
}

.accordion-content ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.accordion-content li {
  margin-bottom: 0.5rem;
}

.accordion-link {
  display: block;
  margin-top: 1rem;
  color: black;
  text-decoration: underline;
  cursor: pointer;
}

.åbningsdage-line {
  display: flex;
  justify-content: space-between;
}
</style>
