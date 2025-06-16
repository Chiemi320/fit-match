<script setup></script>

<template>
  <section class="app-benefits">
    <h3 class="app-benefits__title">Why FitMatch Works</h3>
    <!-- Will be components later -->
    <!-- Card1 -->
    <div class="app-benefits__card">
      <img
        class="app-benefits__image"
        src="@/assets/images/placeholders/placeholder-image.jpg"
        alt="Placeholder Image"
      />
      <div class="app-benefits__content">
        <h4 class="app-benefits__heading">AI-Powered Connections</h4>
        <p class="app-benefits__description">
          Advanced algorithms pair you with trainers who match your fitness goals, preferred workout
          style, and schedule for seamless compatibility.
        </p>
      </div>
    </div>
    <!-- Card2 -->
    <div class="app-benefits__card">
      <img
        class="app-benefits__image"
        src="@/assets/images/placeholders/placeholder-image.jpg"
        alt="Placeholder Image"
      />
      <div class="app-benefits__content">
        <h4 class="app-benefits__heading">FitMatch Certified Trainers</h4>
        <p class="app-benefits__description">
          Connect with elite trainers who've completed our comprehensive certification program,
          ensuring world-class expertise in health and beauty fitness.
        </p>
      </div>
    </div>
    <!-- Card3 -->
    <div class="app-benefits__card">
      <img
        class="app-benefits__image"
        src="@/assets/images/placeholders/placeholder-image.jpg"
        alt="Placeholder Image"
      />
      <div class="app-benefits__content">
        <h4 class="app-benefits__heading">Connect & Grow Together</h4>
        <p class="app-benefits__description">
          A unique ecosystem where fitness enthusiasts find their perfect trainer while aspiring
          trainers build successful careers through our certification pathway.
        </p>
      </div>
    </div>
  </section>
</template>

<style scoped>
.app-benefits {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  background-color: var(--bg-color-secondary);
  padding-block: 4rem;
  padding-inline: var(--body-padding-inline);
}

.app-benefits__card {
  display: flex;
  flex-direction: column;
  overflow: clip;
  border-radius: 1.5rem;
  background-color: var(--bg-color-primary);
}

.app-benefits__content {
  padding: 2rem;
}

.app-benefits__heading {
  margin-bottom: 1rem;
}
</style>
