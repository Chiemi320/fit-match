<script setup>
import { PrimaryButton } from '@/components/buttons/index.js'
import { SecondaryButton } from '@/components/buttons/index.js'
</script>

<template>
  <section class="hero-section">
    <h4 class="hero-section__subtitle">Lorem ipsum dolor</h4>
    <h2 class="hero-section__title">Lorem ipsum dolor sit amet</h2>
    <p class="hero-section__description">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut
      labore et dolore magna aliqua.
    </p>
    <div class="hero-section__buttons">
      <PrimaryButton />
      <SecondaryButton />
    </div>
    <div class="hero-section__label">Featured in</div>
    <div class="hero-section__logos">
      <!-- those are supposed to be img tags -->
      <div class="hero-section__logo">MediaLogo</div>
      <div class="hero-section__logo">MediaLogo</div>
      <div class="hero-section__logo">MediaLogo</div>
      <div class="hero-section__logo">MediaLogo</div>
      <div class="hero-section__logo">MediaLogo</div>
      <div class="hero-section__logo">MediaLogo</div>
    </div>
    <img
      class="hero-section__image"
      src="@/assets/images/placeholders/placeholder-image.jpg"
      alt="Placeholder Image"
    />
  </section>
</template>

<style scoped></style>
