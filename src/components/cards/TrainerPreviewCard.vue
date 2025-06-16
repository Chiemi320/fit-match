<script setup>
import { SmallButton } from '@/components/buttons/index.js'
</script>

<template>
  <div class="trainer-preview-card">
    <img
      class="trainer-preview-card__image"
      src="@/assets/images/placeholders/placeholder-image.jpg"
      alt="Trainer Preview Image"
    />
    <span class="trainer-preview-card__stars">★★★★★</span>
    <h4 class="trainer-preview-card__subtitle">Trainer Name</h4>
    <p class="trainer-preview-card__intro">
      This is a brief description of the trainer, highlighting their expertise and experience.
      Please input something here for the clients.
    </p>
    <!-- Learn Moreを入れる -->
    <SmallButton />
  </div>
</template>

<style scoped>
.trainer-preview-card {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1.25rem;
  padding: 3.38rem 1.5rem 2rem;
  background-color: var(--bg-color-primary);
  border-radius: 6.63rem;
}

.trainer-preview-card__image {
  width: 9.38rem;
  height: 9.38rem;
  border-radius: 50%;
}

.trainer-preview-card__stars {
  font-size: 1.5rem;
  margin-bottom: 0.5rem;
}

.trainer-preview-card__intro {
  margin-bottom: 0.5rem;
}
</style>
