<script setup></script>

<template>
  <section class="app-benefits">
    <div class="app-benefits__container container">
      <h3 class="app-benefits__title">Why FitMatch Works</h3>

      <div class="app-benefits__grid">
        <div class="app-benefits__grid-item">
          <div class="app-benefits__overflow-image">
            <img
              class="app-benefits__image"
              src="@/assets/images/placeholders/placeholder-image.jpg"
              alt="Placeholder Image"
            />
          </div>
        </div>
        <div class="app-benefits__grid-item">
          <div class="app-benefits__content">
            <h4 class="app-benefits__heading">AI-Powered Connections</h4>
            <p class="app-benefits__description description">
              Advanced algorithms pair you with trainers who match your fitness goals, preferred
              workout style, and schedule for seamless compatibility.
            </p>
          </div>
        </div>
        <div class="app-benefits__grid-item grid4">
          <div class="app-benefits__overflow-image is-even">
            <img
              class="app-benefits__image"
              src="@/assets/images/placeholders/placeholder-image.jpg"
              alt="Placeholder Image"
            />
          </div>
        </div>
        <div class="app-benefits__grid-item grid3">
          <div class="app-benefits__content">
            <h4 class="app-benefits__heading">FitMatch Certified Trainers</h4>
            <p class="app-benefits__description description">
              Connect with elite trainers who've completed our comprehensive certification program,
              ensuring world-class expertise in health and beauty fitness.
            </p>
          </div>
        </div>

        <div class="app-benefits__grid-item">
          <div class="app-benefits__overflow-image">
            <img
              class="app-benefits__image"
              src="@/assets/images/placeholders/placeholder-image.jpg"
              alt="Placeholder Image"
            />
          </div>
        </div>
        <div class="app-benefits__grid-item">
          <div class="app-benefits__content">
            <h4 class="app-benefits__heading">Connect & Grow Together</h4>
            <p class="app-benefits__description description">
              A unique ecosystem where fitness enthusiasts find their perfect trainer while aspiring
              trainers build successful careers through our certification pathway.
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.app-benefits {
  padding-block: 4rem;
  background-color: var(--background-secondary);

  @media (min-width: 768px) {
    padding-block: 4rem 10rem;
  }
}
.app-benefits__title {
  margin-bottom: 2rem;

  @media (min-width: 768px) {
    margin-bottom: 4rem;
  }
}

.app-benefits__heading {
  margin-bottom: 1rem;
}

.app-benefits__grid {
  display: flex;
  flex-direction: column;
  gap: 2rem;

  @media (min-width: 768px) {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    gap: 1rem;
  }
}

.app-benefits__grid-item {
  @media (min-width: 768px) {
    position: relative;
    overflow: visible;
    min-height: 350px;

    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding-inline: 2.5rem;
  }
}

.app-benefits__overflow-image {
  @media (min-width: 768px) {
    position: absolute;
    top: -10%;
    left: 0;
    width: 108%;
    height: 120%;
  }
}

.app-benefits__content {
  text-align: center;
}

.app-benefits__overflow-image.is-even {
  @media (min-width: 768px) {
    right: 0;
    left: auto;
  }
}

.app-benefits__image {
  border-radius: 1.5rem;
  object-fit: cover;
  width: 100%;
  height: 100%;
}

.grid3 {
  grid-column: 1;
  grid-row: 2;
}
.grid4 {
  grid-column: 2;
  grid-row: 2;
}

.description {
  margin-bottom: 2rem;
}
</style>
