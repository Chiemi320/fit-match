<script setup>
import BaseLink from '@/components/BaseLink.vue'
</script>

<template>
  <header class="app-header">
    <h1><RouterLink class="app-header__link" to="/">Logo</RouterLink></h1>
    <ul class="app-header__list show-only-desktop">
      <li class="app-header__item">
        <RouterLink class="app-header__link" to="/">Home</RouterLink>
      </li>
      <li class="app-header__item">
        <RouterLink class="app-header__link" to="/about">About Us</RouterLink>
      </li>
      <li class="app-header__item">
        <RouterLink class="app-header__link" to="/contact">Contact</RouterLink>
      </li>
    </ul>
    <div class="app-header__btns show-only-desktop">
      <BaseLink to="/login" variant="login">Login</BaseLink>
      <BaseLink to="/signup" variant="signup">Sign up</BaseLink>
    </div>
    <button class="app-header__ham-menu show-only-mobile">
      <span class="app-header__ham-line"></span>
      <span class="app-header__ham-line"></span>
      <span class="app-header__ham-line"></span>
    </button>
  </header>
</template>

<style lang="scss" scoped>
.app-header {
  // Header variables
  --header-height: #{$header-height};
  --header-padding-inline: #{$header-padding-inline};
  --header-z-index: #{$header-z-index};

  // Hamburger menu variables
  --ham-line-color: #{$ham-line-color};

  position: fixed;
  top: 0;
  left: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: var(--header-z-index);
  width: 100%;
  height: var(--header-height);
  padding-inline: var(--header-padding-inline);
  border-bottom: 1px solid #2d2d2d;
}

.app-header__link {
  display: inline-block;
  width: 100%;
  height: 100%;
  padding: 0.5rem;
}

.app-header__list {
  display: flex;
  justify-content: center;
  gap: 1rem;
}

.app-header__btns {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 0.5rem;
}

.app-header__ham-menu {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  width: var(--btn-size-l);
  height: var(--btn-size-l);
  padding: 0.8rem 0.5rem;
}

.app-header__ham-line {
  display: block;
  width: 100%;
  height: 3px;
  background-color: var(--ham-line-color);
}
</style>
