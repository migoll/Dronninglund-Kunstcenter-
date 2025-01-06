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
  header {
    background-color: #333;
    color: white;
    padding: 1rem 0;
  }
  </style>
  