<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style>
:root {
  /* Cores */

  --black: #1c232b;
  --gray: #6c7289;
  --cream: #f2eae2;
  --white: #ffffff;
  --green-500: #3d8168;
  --green-700: #1a4032;

  /* Tipografia */

  --text-preset-1: 700 32px/1 'Fraunces', serif;
  --text-preset-1-letter-spacing: 0;
  --text-preset-2: 700 14px/1.1 'Montserrat', sans-serif;
  --text-preset-2-letter-spacing: 0;
  --text-preset-3: 500 14px 1.6 'Montserrat', sans-serif;
  --text-preset-3-letter-spacing: 0;
  --text-preset-4: 500 12px 1.2 'Montserrat', sans-serif;
  --text-preset-4-letter-spacing: 5px;
  --text-preset-5: 500 13px 1.2 'Montserrat', sans-serif;
  --text-preset-5-letter-spacing: 0;

  /* Spacing */

  --spacing-50: 4px;
  --spacing-100: 8px;
  --spacing-200: 16px;
  --spacing-300: 24px;
  --spacing-400: 32px;
  --spacing-500: 40px;
}

.text-preset-1 {
  font: var(--text-preset-1);
  letter-spacing: var(--text-preset-1-letter-spacing);
  color: var(--black);
}

.text-preset-2 {
  font: var(--text-preset-2);
  letter-spacing: var(--text-preset-2-letter-spacing);
  color: var(--black);
}

.text-preset-3 {
  font: var(--text-preset-3);
  letter-spacing: var(--text-preset-3-letter-spacing);
  color: var(--gray);
}

.text-preset-4 {
  font: var(--text-preset-4);
  letter-spacing: var(--text-preset-4-letter-spacing);
  color: var(--gray);
}

.text-preset-5 {
  font: var(--text-preset-5);
  letter-spacing: var(--text-preset-5-letter-spacing);
  color: var(--gray);
  text-decoration: line-through;
}
</style>
