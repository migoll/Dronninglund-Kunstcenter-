<template>
  <footer class="footer">
    <div class="footer-container">
      <div class="footer-info">
        <p>THORUP HEDEVEJ 1</p>
        <p>9330 DRONNINGLUND</p>
        <p>TLF. 9647 6600</p>
        <div class="social-icons">
          <img
            class="search-icon"
            src="~assets/icons/instagram-brands-solid.svg"
            alt=""
          />
          <img
            class="search-icon"
            src="~assets/icons/square-facebook-brands-solid.svg"
            alt=""
          />
        </div>
      </div>

      <div class="footer-logo">
        <img
          src="@/assets/images/logo/DRK-logo.svg"
          alt="Dronninglund Kunstcenter Logo"
        />
      </div>

      <div class="footer-login">
        <p>Er du medarbejder?</p>
        <button class="login-button">Login</button>
      </div>
    </div>
  </footer>
</template>

<script setup></script>

<style scoped>
.footer {
  background-color: var(--primary-black);
  color: var(--primary-white);
  padding: 2rem 0;
}

.footer-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1080px;
  margin: 0 auto;
}

.footer-info {
  text-align: left;
}

.footer-info p {
  margin: 5px 0;
}

.social-icons {
  display: flex;
  gap: 15px;
  margin-top: 10px;
}

.social-icons img {
  width: 35px;
  height: 35px;
}

.footer-logo {
  text-align: center;
}

.footer-login {
  text-align: right;
}

.login-button {
  background: none;
  border: 3px solid var(--primary-white);
  color: var(--primary-white);
  padding: 0.5rem 1rem;
  border-radius: 6px;
  cursor: pointer;
  font-size: 1rem;
  width: stretch;
}
</style>
