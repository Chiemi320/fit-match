<script setup></script>

<template>
  <section class="review-preview">
    <!-- Will be components later -->
    <!-- Review1 -->
    <div class="review-preview__review">
      <img
        class="review-preview__icon"
        src="@/assets/images/placeholders/placeholder-image.jpg"
        alt="Review Preview Icon"
      />
      <div class="review-preview__content">
        <p class="review-preview__voice">"Paste a voice here. The longer the better!"</p>
        <div class="review-preview__name">Reviewer Name</div>
        <span class="review-preview__stars">★★★★★</span>
      </div>
    </div>

    <div class="review-preview__review">
      <img
        class="review-preview__icon"
        src="@/assets/images/placeholders/placeholder-image.jpg"
        alt="Review Preview Icon"
      />
      <div class="review-preview__content">
        <p class="review-preview__voice">"Paste a voice here. The longer the better!"</p>
        <div class="review-preview__name">Reviewer Name</div>
        <span class="review-preview__stars">★★★★★</span>
      </div>
    </div>

    <div class="review-preview__review">
      <img
        class="review-preview__icon"
        src="@/assets/images/placeholders/placeholder-image.jpg"
        alt="Review Preview Icon"
      />
      <div class="review-preview__content">
        <p class="review-preview__voice">"Paste a voice here. The longer the better!"</p>
        <div class="review-preview__name">Reviewer Name</div>
        <span class="review-preview__stars">★★★★★</span>
      </div>
    </div>
  </section>
</template>

<style scoped>
.review-preview {
  display: flex;
  flex-direction: column;
  gap: 4.68rem;
  padding-block: 2.5rem;
  padding-inline: var(--body-padding-inline);
}

.review-preview__review {
  display: flex;
  padding: 1.5rem;
  gap: 1rem;
  border: 1px solid var(--bg-color-secondary);
  border-radius: 0.5rem;
}

.review-preview__icon {
  width: var(--icon-size-medium);
  height: var(--icon-size-medium);
  border-radius: 50%;
}

.review-preview__content {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
}

.review-preview__voice {
  font-size: 1.2rem;
}

.review-preview__stars {
  font-size: 1.25rem;
}
</style>
