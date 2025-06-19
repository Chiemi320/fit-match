<script setup>
import BaseLink from '@/components/BaseLink.vue'
</script>

<template>
  <section class="hero-section">
    <div class="hero-section__container">
      <div class="hero-section__content">
        <h4 class="hero-section__subtitle">Perfectly Paired Fitness</h4>
        <h2 class="hero-section__title">Your Trainer Match Awaits</h2>
        <p class="hero-section__description">
          No more trial and error. Find trainers who match your goals, schedule, and training style
          perfectly.
        </p>
        <BaseLink to="/signup" variant="signup" class="hero-section__btn">Start Today</BaseLink>
        <div class="hero-section__label">Featured in</div>
        <div class="hero-section__logos">
          <!-- Replace the placeholder logo with mockups -->
          <div class="hero-section__logo logo">BigLogo</div>
          <div class="hero-section__logo logo">BigLogo</div>
          <div class="hero-section__logo logo">BigLogo</div>
          <div class="hero-section__logo logo">BigLogo</div>
          <div class="hero-section__logo logo">BigLogo</div>
        </div>
      </div>
      <div class="hero-section__image-container">
        <img
          class="hero-section__image"
          src="@/assets/images/placeholders/mockup-mobile-small.png"
          alt="FitMatch connects people with fitness goals to certified trainers and fitness enthusiasts."
        />
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.hero-section {
  width: 100%;
  padding-block: 9.7rem 3.6rem;

  @media (min-width: 768px) {
    display: flex;
    flex-direction: row;
    justify-content: center;
    padding-block: 6rem;
  }
}

.hero-section__container {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-inline: var(--padding-inline);
  max-width: var(--container-m);

  @media (min-width: 768px) {
    flex-direction: row;
    align-items: flex-start;
    gap: 8vw;
  }
}

.hero-section__content {
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  max-width: 500px;
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
.hero-section__description,
.hero-section__logos {
  margin-bottom: 2.25rem;
}

.hero-section__btn {
  width: 100%;
  margin-bottom: 2.7rem;

  @media (min-width: 768px) {
    width: 18rem;
  }
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
  max-width: 400px;
  height: auto;
  border-radius: 1.5rem;
}

/* Logos are placeholders */
.hero-section__logo {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0 0.5rem;
}

.logo {
  font-size: 1.8rem;
  font-weight: bold;
  font-style: italic;
}
</style>
