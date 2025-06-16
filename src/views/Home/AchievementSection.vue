<script setup></script>

<template>
  <section class="achievement">
    <h3 class="achievement__title">Achievements</h3>
    <div class="achievement__content">
      <div class="achievement__number">24+</div>
      <p class="achievement__description">Years of combined experience in the fitness industry</p>
    </div>
    <div class="achievement__content">
      <div class="achievement__number">17M</div>
      <p class="achievement__description">Years of combined experience in the fitness industry</p>
    </div>
    <div class="achievement__content">
      <div class="achievement__number">+95%</div>
      <p class="achievement__description">Years of combined experience in the fitness industry</p>
    </div>
  </section>
</template>

<style scoped>
.achievement {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  padding-block: 4rem;
  padding-inline: var(--body-padding-inline);
}

.achievement__title {
  text-align: center;
}

.achievement__content {
  padding: 2rem;
  border-radius: 1.5rem;
  background-color: var(--bg-color-secondary);
}

.achievement__number {
  font-size: 2.64rem;
  font-weight: 700;
  margin-bottom: 1rem;
}

.achievement__description {
  font-size: 1.2rem;
}
</style>
