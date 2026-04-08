<script setup>
import NavBar from '../components/NavBar.vue'
</script>

<template>
  <div class="page">
    <NavBar />
    <main class="content">
      <h1>Heat Vulnerability Map</h1>
      <p>Coming soon.</p>
    </main>
  </div>
</template>

<style scoped>
.page {
  min-height: 100vh;
}

.content {
  max-width: var(--max-width);
  margin: 0 auto;
  padding: 4rem 2rem;
}
</style>
