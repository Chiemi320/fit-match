<script setup></script>

<template>
  <section class="trainer-preview">
    <h3 class="trainer-preview__title">Trainer Preview</h3>
    <button type="button" class="trainer-preview__btn trainer-preview__btn--prev">&lt;</button>
    <button type="button" class="trainer-preview__btn trainer-preview__btn--next">&gt;</button>

    <div class="trainer-preview__carousel">
      <div class="trainer-preview__items">
        <!-- will be components later -->
        <!-- Card1 -->
        <div class="trainer-preview__item">
          <img
            class="trainer-preview__image"
            src="@/assets/images/placeholders/placeholder-image.jpg"
            alt="Trainer Preview Image"
          />
          <span>★★★★★</span>
          <h4 class="trainer-preview__subtitle">Trainer Name</h4>
          <p class="trainer-preview__intro">
            This is a brief description of the trainer, highlighting their expertise and experience.
          </p>
          <button type="button" class="trainer-preview__button">Learn More</button>
        </div>
        <!-- Card2 -->
        <div class="trainer-preview__item">
          <img
            class="trainer-preview__image"
            src="@/assets/images/placeholders/placeholder-image.jpg"
            alt="Trainer Preview Image"
          />
          <span>★★★★★</span>
          <h4 class="trainer-preview__subtitle">Trainer Name</h4>
          <p class="trainer-preview__intro">
            This is a brief description of the trainer, highlighting their expertise and experience.
          </p>
          <button type="button" class="trainer-preview__button">Learn More</button>
        </div>
        <!-- Card3 -->
        <div class="trainer-preview__item">
          <img
            class="trainer-preview__image"
            src="@/assets/images/placeholders/placeholder-image.jpg"
            alt="Trainer Preview Image"
          />
          <span>★★★★★</span>
          <h4 class="trainer-preview__subtitle">Trainer Name</h4>
          <p class="trainer-preview__intro">
            This is a brief description of the trainer, highlighting their expertise and experience.
          </p>
          <button type="button" class="trainer-preview__button">Learn More</button>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped></style>
