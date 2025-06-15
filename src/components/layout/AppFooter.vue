<script setup></script>

<template>
  <footer class="app-footer">
    <h1><RouterLink class="app-footer__link" to="/">Logo</RouterLink></h1>
    <nav class="app-footer__nav">
      <section class="app-footer__nav-section">
        <h5 class="app-footer__nav-title">Company</h5>
        <ul class="app-footer__nav-list">
          <li><RouterLink to="/about">About</RouterLink></li>
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
      <a href="#" class="app-footer__social-link">Facebook</a>
      <a href="#" class="app-footer__social-link">Twitter</a>
      <a href="#" class="app-footer__social-link">Instagram</a>
    </div>

    <div class="app-footer__copyright">&copy; 2025 Your Company Name. All rights reserved.</div>
  </footer>
</template>

<style scoped></style>
