<template>
  <section class="forside-hero">
    <img src="" alt="" />
    <img src="" alt="" />
    <img src="" alt="" />
  </section>
  <div class="åbningstider-box">
    <div>
      <h3>Åbningstider</h3>
      <ul>
        <li>Mandag: Lukket</li>
        <li>Tirsdag - Fredag: 13:00 - 17:00</li>
        <li>Lørdag - Søndag: 11:00 - 17:00</li>
      </ul>
    </div>
  </div>
  <section class="forside-entry-points center-section">
    <div class="entry-points-1"></div>
    <div class="entry-points-2"></div>
    <div class="entry-points-3"></div>
  </section>
  <section class="om-os">
    <div class="om-os-info">
      <h2>Om Dronninglund Kunstcenter</h2>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut et massa mi.
        Aliquam in hendrerit urna. Pellentesque sit amet sapien fringilla,
        mattis ligula consectetur, ultrices mauris. Maecenas vitae mattis
        tellus. Nullam quis imperdiet augue. Vestibulum auctor ornare leo, non
        suscipit magna interdum eu. Curabitur pellentesque nibh nibh, at maximus
        ante fermentum sit amet. Pellentesque commodo lacus at sodales
      </p>
      <p>
        uam in hendrerit urna. Pellentesque sit amet sapien fringilla, mattis
        ligula consectetur, ultrices mauris. Maecenas vitae mattis tellus.
        Nullam quis imperdiet augue. Vestibulum auctor ornare leo, non suscipit
        magna interdum eu. Curabitur pellentesque nibh nibh, at maximus ante
        fermentum sit amet.
      </p>
      <button class="reverse-button-white">Læs mere om os</button>
    </div>
    <img src="" alt="" />
  </section>
  <section class="forside-sponsors">
    <img src="" alt="" />
    <img src="" alt="" />
    <img src="" alt="" />
    <img src="" alt="" />
    <img src="" alt="" />
    <img src="" alt="" />
    <img src="" alt="" />
    <img src="" alt="" />
  </section>
  <section class="forside-nyhedsbrev">
    <div class="forside-nyhedsbrev center-section">
      <h3>Vores Nyhedsbrev</h3>
      <p>
        Tildmeld dig vores nyhedsbrev for at blive opdateret om nye
        begivenheder, udstillinger og unikke tilbud.
      </p>
      <div class="tilmeld-container">
        <input
          type="email"
          placeholder="john_doe@mail.com"
          class="email-input"
        />
        <button class="tilmeld-button">Tilmeld</button>
      </div>
    </div>
  </section>
  <div class="divider-hr"></div>
</template>

<script setup></script>

<style scoped>
.forside-hero {
  display: flex;
  width: 100%;
}
.forside-hero img {
  background-color: yellow;
  border: 3px solid red;
  flex-grow: 1;
  height: 400px;
}

.forside-entry-points {
  display: flex;
  justify-content: space-between;
}

.entry-points-1,
.entry-points-2,
.entry-points-3 {
  width: 250px;
  height: 350px;
  background-color: blue;
  border: 3px solid green;
}

.om-os {
  background-color: black;
  color: white;
  display: flex;
}

.om-os-info,
.om-os img {
  flex: 0 0 50%;
  height: 400px;
}

.om-os img {
  object-fit: cover;
  background-color: green;
  border: 3px solid red;
}

.reverse-button-white {
  background: none;
  border: 3px solid white;
  color: white;
  padding: 0.5rem 1.5rem;
  border-radius: 6px;
  cursor: pointer;
  font-size: 1rem;
}

.tilmeld-container {
  display: flex;
  width: 100%;
  max-width: 400px;
  border-radius: 6px;
  overflow: hidden;
}

.email-input {
  flex: 1;
  border: none;
  padding: 10px 15px;
  font-size: 16px;
  color: #666;
  outline: none;
}

.email-input::placeholder {
  color: #aaa;
}

.tilmeld-button {
  background-color: #2da18e;
  color: white;
  border: none;
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
  transition: background-color 0.2s ease;
}

.tilmeld-button:hover {
  background-color: var(--primary-main);
}

.forside-nyhedsbrev {
  background-color: var(--primary-black);
  color: var(--primary-white);
  padding: 1rem 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
