<template>
  <header class="header">
    <div class="top-section">
      <div class="search">
        <h2>Search icon</h2>
      </div>
      <div class="logo">
        <img
          src="@/assets/images/logo/DRK-logo.svg"
          alt="Dronninglund Kunstcenter Logo"
        />
      </div>
      <div class="buttons">
        <button class="language-button">DA</button>
        <button class="ticket-button">Køb billet</button>
      </div>
    </div>

    <div class="divider-hr"></div>

    <nav class="bottom-section">
      <div class="nav-container">
        <div class="nav-list-left">
          <a href="/">Forside</a>
          <a href="/udstillinger">Udstillinger</a>
          <a href="/begivenheder">Begivenheder</a>
        </div>
        <div class="divider-vr"></div>
        <div class="nav-list-right">
          <a href="/se-mere">Se mere</a>
        </div>
      </div>
    </nav>
  </header>
  </template>
  
  <script setup>
  </script>

<style scoped>
.header {
  background-color: var(--primary-black);
  color: var(--primary-white);
}

.top-section {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  align-items: center;
  padding: 1rem 2rem;
  max-width: 1080px;
  margin: 0 auto;
}

.bottom-section {
  display: flex;
  justify-content: center;
}

.search img {
  width: 20px;
  height: 20px;
  justify-self: start;
}

.logo {
  text-align: center;
}

.logo img {
  margin: 0 auto;
}

.buttons {
  display: flex;
  gap: 10px;
  justify-self: end;
}

.language-button,
.ticket-button {
  background-color: var(--primary-white);
  color: var(--primary-black);
  border: none;
  padding: 0.5rem 1rem;
  border-radius: 6px;
  cursor: pointer;
  font-size: 1rem;
}

.divider-hr {
  height: 1px;
  background-color: var(--primary-white);
  opacity: 0.2;
  max-width: 1080px;
  margin: 0 auto;
}

.nav-container {
  display: flex;
  align-items: center;
  padding: 1rem 0;
}

.nav-list-left,
.nav-list-right {
  display: flex;
  gap: 20px;
}

.divider-vr {
  width: 1px;
  height: 35px;
  background-color: var(--primary-white);
  opacity: 0.5;
  margin: 0 20px;
}

.nav-list-left a,
.nav-list-right a {
  color: var(--primary-white);
  text-decoration: none;
  font-size: 16px;
}
</style>
