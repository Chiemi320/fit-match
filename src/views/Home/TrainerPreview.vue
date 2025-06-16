<script setup>
import { TrainerPreviewCard } from '@/components/cards/index.js'
</script>

<template>
  <section class="trainer-preview">
    <h3 class="trainer-preview__title">Meet Your Future Trainers</h3>
    <button type="button" class="trainer-preview__btn trainer-preview__btn--prev">
      <span>&lt;</span>
    </button>
    <button type="button" class="trainer-preview__btn trainer-preview__btn--next">
      <span>&gt;</span>
    </button>

    <div class="trainer-preview__carousel">
      <div class="trainer-preview__items">
        <TrainerPreviewCard class="trainer-preview__item" />
        <TrainerPreviewCard class="trainer-preview__item" />
        <TrainerPreviewCard class="trainer-preview__item" />
      </div>
    </div>
  </section>
</template>

<style scoped>
.trainer-preview {
  position: relative;
  padding-block: 4rem;
  background-color: var(--bg-color-secondary);
}

.trainer-preview__title {
  text-align: center;
  margin-bottom: 3rem;
}

.trainer-preview__btn {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  display: flex;
  align-items: center;
  justify-content: center;
  width: 3rem;
  height: 3rem;
  line-height: 1;
  font-size: 1.5rem;
  padding-bottom: 0.25rem;
  background-color: var(--btn-primary);
  border-radius: 50%;
}

.trainer-preview__carousel {
  overflow: auto;
  scroll-snap-type: x mandatory;
  width: 100%;
}

.trainer-preview__items {
  display: flex;
  justify-content: flex-start;
  width: fit-content;
}

.trainer-preview__item {
  flex: 0 0 90vw;
  flex-shrink: 0;
  scroll-snap-align: center;
  margin-inline: var(--body-padding-inline);
}
</style>
