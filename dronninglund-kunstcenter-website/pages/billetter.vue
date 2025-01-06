<template>
  <section class="center-section">
    <h1>Entrebillet</h1>
    <h3>Adgangsbillet til Dronninglund Kunstcenter</h3>
    <div class="voksen-billet">
      <div>
        <p>Voksen 18+</p>
        <p>Børn under 15 er gratis</p>
      </div>
      <div class="ticket-counter">
        <p>80 kr</p>
        <button>-</button>
        <p>80 kr</p>
        <button>+</button>
      </div>
    </div>
    <button class="black-button">Køb</button>
  </section>
  <div class="divider-hr"></div>
  <section class="center-section">
    <h1>Gruppebillet</h1>
    <div class="voksen-billet">
      <p>
        For store grupper kontakt Dronninglund Kunstcenter for grupperabat over
        15 personer
      </p>
    </div>
    <button class="reverse-button-black">Kontakt os</button>
  </section>
  <div class="divider-hr"></div>
</template>

<script setup></script>
<style scoped>
.ticket-counter {
  display: flex;
  flex-direction: row;
  gap: 1rem;
  align-items: center;
}

.ticket-counter button {
  width: 40px;
  height: 40px;
}

.voksen-billet {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>
