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
:root {
  /* Global style variables */
  --body-padding: #{$body-padding};
  --body-padding-inline: #{$body-padding-inline};

  --icon-size-medium: #{$icon-size-medium};

  /* Color variables */
  --text-white: #{$text-light};
  --text-primary: #{$text-primary};

  --bg-color-primary: #{$background-primary};
  --bg-color-secondary: #{$background-secondary};
  --bg-color-dark: #{$background-dark};

  /* Font family variables */
  --font-family-display: #{$font-display};

  /*下からチェック済み*/
}

/* Global styles for the app */
.main-content {
  margin-top: 4rem;
}

/* Utilities style */
.show-only-mobile {
  @media (min-width: 768px) {
    display: none !important;
  }
}

.show-only-desktop {
  @media (max-width: 767px) {
    display: none !important;
  }
}

/* Boostrap icon size */
.bi {
  font-size: 1.8rem;
}
</style>
