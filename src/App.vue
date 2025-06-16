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

  /* Color variables */
  --text-white: #{$text-light};
  --btn-primary: #{$primary-dark};
  --bg-color-primary: #{$background-primary};
  --bg-color-secondary: #{$background-secondary};
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
</style>
