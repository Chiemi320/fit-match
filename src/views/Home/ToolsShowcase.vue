<script setup>
import { SmallButton } from '@/components/buttons/index.js'
</script>

<template>
  <section class="tools-showcase">
    <h3 class="tools-showcase__title">Anti-Quit Technology</h3>
    <!-- Tool Section1 -->
    <section class="tools-showcase__section">
      <img
        class="tools-showcase__image tools-showcase__image--right"
        src="@/assets/images/placeholders/placeholder-image.jpg"
        alt="Tools Showcase Image"
      />
      <h4 class="tools-showcase__subtitle">Progress Momentum Tracker</h4>
      <p class="tools-showcase__description">
        Visual progress mapping and milestone celebrations keep you motivated. Our smart analytics
        identify potential quit points and automatically trigger personalized encouragement to
        maintain your fitness momentum.
      </p>
      <!-- See How It Worksといれる -->
      <SmallButton />
    </section>
    <!-- Tool Section2 -->
    <section class="tools-showcase__section">
      <img
        class="tools-showcase__image tools-showcase__image--left"
        src="@/assets/images/placeholders/placeholder-image.jpg"
        alt="Tools Showcase Image"
      />
      <h4 class="tools-showcase__subtitle">Accountability Partner System</h4>
      <p class="tools-showcase__description">
        Never train alone again. Our built-in buddy system pairs you with accountability partners
        and sends smart reminders, progress check-ins, and motivational nudges when you need them
        most.
      </p>
      <!-- Find Your Partnerといれる -->
      <SmallButton />
    </section>
    <!-- Tool Section Summary -->
    <section class="tools-showcase__footer">
      <div class="tools-showcase__footer-title">
        Built to Beat<br />
        the 90% Quit Rate
      </div>
      <p class="tools-showcase__footer-description">
        Most people quit fitness programs within 3 months. Our scientifically-backed retention tools
        use behavioral psychology and AI insights to keep you engaged, motivated, and on track for
        long-term success.
      </p>
    </section>
  </section>
</template>

<style scoped>
.tools-showcase {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-block: 5.5rem;
  padding-inline: var(--body-padding-inline);
}

.tools-showcase__title {
  width: 100%;
  text-align: right;
  margin-bottom: 2rem;
}

.tools-showcase__section {
  display: flex;
  flex-direction: column;
  margin-bottom: 4.5rem;
}

.tools-showcase__image {
  margin-inline: calc(var(--body-padding-inline) * -1);
  margin-bottom: 1.5rem;
}

.tools-showcase__image--right {
  align-self: flex-end;
  border-radius: 1.5rem 0 0 1.5rem;
}

.tools-showcase__image--left {
  align-self: flex-start;
  border-radius: 0 1.5rem 1.5rem 0;
}

.tools-showcase__subtitle {
  margin-bottom: 1rem;
}

.tools-showcase__description {
  margin-bottom: 1.5rem;
}

.tools-showcase__footer {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
  width: 85%;
}

.tools-showcase__footer-title {
  font-size: 1.56rem;
  font-weight: 300;
  margin-bottom: 1rem;
}
</style>
