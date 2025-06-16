<script setup>
import AppHeader from '@/components/layout/AppHeader.vue'
import AppFooter from '@/components/layout/AppFooter.vue'
</script>

<template>
  <AppHeader />
  <main class="main-content">
    <RouterView />
  </main>
  <AppFooter />
</template>

<style lang="scss">
@use './assets/abstracts/variables.scss' as *;

:root {
  /* Global style variables */
  --body-padding: #{$body-padding};
  --body-padding-inline: #{$body-padding-inline};

  --icon-size-medium: #{$icon-size-medium};

  /* Color variables */
  --text-white: #{$text-light};
  --text-primary: #{$text-primary};
  --btn-primary: #{$dark-gray};
  --bg-color-primary: #{$background-primary};
  --bg-color-secondary: #{$background-secondary};
  --bg-color-dark: #{$background-dark};

  /* Font family variables */
  --font-family-display: #{$font-display};
}

/* Global styles for the app */
.main-content {
  margin-top: 4rem;
}

/* General button styles */
.btn {
  display: block;
  border-radius: 2rem;
  padding-block: 0.57rem;
  text-align: center;
}

/* Boostrap icon size */
.bi {
  font-size: 1.8rem;
}
</style>
