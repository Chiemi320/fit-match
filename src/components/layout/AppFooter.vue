<script setup></script>

<template>
  <footer class="app-footer">
    <h1><RouterLink to="/" class="app-footer__logo">Logo</RouterLink></h1>
    <nav class="app-footer__nav">
      <section class="app-footer__nav-section">
        <h5 class="app-footer__nav-title">Company</h5>
        <ul class="app-footer__nav-list">
          <li><RouterLink to="/about">About Us</RouterLink></li>
          <li><RouterLink to="/blog">Blog</RouterLink></li>
        </ul>
      </section>

      <section class="app-footer__nav-section">
        <h5 class="app-footer__nav-title">Support</h5>
        <ul class="app-footer__nav-list">
          <li><RouterLink to="/contact">Contact</RouterLink></li>
          <li><RouterLink to="/faq">FAQ</RouterLink></li>
        </ul>
      </section>

      <section class="app-footer__nav-section">
        <h5 class="app-footer__nav-title">Offer</h5>
        <ul class="app-footer__nav-list">
          <li><RouterLink to="/tools">Tools</RouterLink></li>
          <li><RouterLink to="/trainers">Trainers</RouterLink></li>
          <li><RouterLink to="/become-a-trainer">Become a Trainer</RouterLink></li>
        </ul>
      </section>
    </nav>

    <div class="app-footer__socials">
      <a href="#" class="app-footer__social-link"><i class="bi bi-facebook"></i></a>
      <a href="#" class="app-footer__social-link"><i class="bi bi-twitter-x"></i></a>
      <a href="#" class="app-footer__social-link"><i class="bi bi-instagram"></i></a>
      <a href="#" class="app-footer__social-link"><i class="bi bi-threads"></i></a>
      <a href="#" class="app-footer__social-link"><i class="bi bi-youtube"></i></a>
    </div>

    <div class="app-footer__copyright">&copy;2025 All rights reserved.</div>
  </footer>
</template>

<style scoped>
.app-footer {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  padding-block: 2rem;
  padding-inline: var(--body-padding-inline);
  background-color: var(--bg-color-dark);
  color: var(--text-white);
}

.app-footer__logo {
  display: inline-block;
  padding: 0.8rem 0.8rem 0.8rem 0;
}

.app-footer__nav {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 3rem 1rem;
  margin-bottom: 3rem;
}

.app-footer__nav-section {
  width: 100%;
  font-size: 1.5rem;
  line-height: 1.4;
}

.app-footer__nav-title {
  margin-bottom: 0.5rem;
}

.app-footer__nav-list a {
  display: block;
  width: 100%;
  padding-block: 0.5rem;
}

.app-footer__socials {
  display: flex;
  justify-content: center;
  gap: 0.5rem;
}

.app-footer__social-link {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 3rem;
  height: 3rem;
  border-radius: 50%;
  background-color: var(--bg-color-secondary);
  color: var(--text-primary);
}

.app-footer__copyright {
  align-self: center;
  max-width: 80%;
}
</style>
