<script setup>
import { PrimaryButton } from '@/components/buttons/index.js'
import { SecondaryButton } from '@/components/buttons/index.js'
</script>

<template>
  <section class="join-us">
    <div class="join-us__text-wrapper">
      <h3 class="join-us__title">Join Us</h3>
      <p class="join-us__message">
        Join our community of fitness enthusiasts and professionals. Whether you're a beginner or an
        experienced athlete, we have something for everyone.
      </p>
    </div>
    <div class="join-us__buttons">
      <PrimaryButton />
      <SecondaryButton />
    </div>
    <img
      class="join-us__image"
      src="@/assets/images/placeholders/placeholder-image.jpg"
      alt="Placeholder Image"
    />
  </section>
</template>

<style scoped>
.join-us {
  display: flex;
  flex-direction: column;
  gap: 2.38rem;
  width: 100%;
  padding-block: 5rem;
  padding-inline: var(--body-padding-inline);
  background-color: var(--bg-color-secondary);
  text-align: center;
}

.join-us__text-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
}

.join-us__title {
  font-size: 1.875rem;
}

.join-us__message {
  width: 90%;
}

.join-us__buttons {
  display: flex;
  flex-direction: column;
  gap: 0.625rem;
  width: 100%;
}

.join-us__image {
  border-radius: 1.5rem;
}
</style>
