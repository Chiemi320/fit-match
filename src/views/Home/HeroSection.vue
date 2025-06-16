<script setup>
import { PrimaryButton } from '@/components/buttons/index.js'
import { SecondaryButton } from '@/components/buttons/index.js'
</script>

<template>
  <section class="hero-section">
    <h4 class="hero-section__subtitle">Perfectly Paired Fitness</h4>
    <h2 class="hero-section__title">Your Trainer Match Awaits</h2>
    <p class="hero-section__description">
      No more trial and error. Find trainers who match your goals, schedule, and training style
      perfectly.
    </p>
    <div class="hero-section__buttons">
      <PrimaryButton />
      <SecondaryButton />
    </div>
    <div class="hero-section__label">Featured in</div>
    <div class="hero-section__logos">
      <!-- those are supposed to be img tags -->
      <div class="hero-section__logo logo1">MediaLogo</div>
      <div class="hero-section__logo logo2">Mock</div>
      <div class="hero-section__logo logo3">Logo<br />Mocked</div>
      <div class="hero-section__logo logo4">BigLogo</div>
      <div class="hero-section__logo logo5">ImageHere</div>
      <div class="hero-section__logo logo6">Logo</div>
    </div>
    <img
      class="hero-section__image"
      src="@/assets/images/placeholders/placeholder-image.jpg"
      alt="Placeholder Image"
    />
  </section>
</template>

<style scoped>
.hero-section {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  padding-block: 9.7rem 3.6rem;
  padding-inline: var(--body-padding-inline);
}

.hero-section__subtitle {
  font-size: 1.5rem;
  margin-bottom: 1.1rem;
}

.hero-section__title {
  font-size: 2.8rem;
  font-weight: bold;
  line-height: 1.3;
  margin-bottom: 2.6rem;
}
.hero-section__description {
  margin-bottom: 2.25rem;
}

.hero-section__buttons {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  width: 100%;
  margin-bottom: 2.25rem;
}

.hero-section__label {
  width: 100%;
  font-size: 1.37rem;
  text-align: left;
  margin-bottom: 0.7rem;
}

.hero-section__logos {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin-bottom: 2.25rem;
}

.hero-section__image {
  width: 100%;
  height: auto;
  border-radius: 1.5rem;
}

/* Logos are placeholders, replace with actual img tags */
.hero-section__logo {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0 0.5rem;
}

.logo1 {
  font-size: 1.2rem;
  font-weight: bold;
}

.logo2 {
  letter-spacing: 0.1rem;
  font-size: 1.2rem;
}

.logo3 {
  font-size: 1.2rem;
  line-height: 1.2;
  font-style: italic;
}

.logo4 {
  font-size: 1.8rem;
  font-weight: bold;
  font-style: italic;
}

.logo5 {
  font-size: 1.4rem;
  text-transform: uppercase;
}

.logo6 {
  font-size: 1.5rem;
  font-weight: 500;
}
</style>
