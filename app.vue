<script setup lang="ts"></script>

<template>
  <div class="site">
    <NuxtPage />
  </div>
</template>

<style lang="scss">
:root {
  --primary: #346ace;
  --primary-light: #dfeaff;
  --primary-dark: #2853a1;

  --site-width: 1280px;
}

*,
*:before,
*:after {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Oxygen,
    Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  font-display: optional;

  .site {
    min-height: 100vh;
  }
}
</style>
