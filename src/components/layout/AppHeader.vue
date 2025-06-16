<script setup></script>

<template>
  <header class="app-header">
    <h1><RouterLink class="app-header__link" to="/">Logo</RouterLink></h1>
    <button class="app-header__ham-menu">
      <span class="app-header__ham-line"></span>
      <span class="app-header__ham-line"></span>
      <span class="app-header__ham-line"></span>
    </button>
  </header>
</template>

<style scoped>
.app-header {
  position: fixed;
  top: 0;
  left: 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
  height: 4rem;
  padding: 0 1rem;
  border-bottom: 1px solid #2d2d2d;
}

.app-header__link {
  display: inline-block;
  width: 100%;
  height: 100%;
  padding: 0.5rem;
}

.app-header__ham-menu {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  width: 3rem;
  height: 3rem;
  padding: 0.8rem 0.5rem;
}

.app-header__ham-line {
  display: block;
  width: 100%;
  height: 3px;
  background-color: #fff;
}
</style>
