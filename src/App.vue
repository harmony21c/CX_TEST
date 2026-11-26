<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <nav class="nav">
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/test">Test</RouterLink>
  </nav>

  <RouterView />
</template>

<style scoped>
.nav {
  display: flex;
  gap: 1rem;
  padding: 1rem 1.5rem;
  border-bottom: 1px solid #e2e8f0;
}

.nav a {
  color: #334155;
  text-decoration: none;
}

.nav a.router-link-active {
  color: #42b883;
  font-weight: 600;
}
</style>
