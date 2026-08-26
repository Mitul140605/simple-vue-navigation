<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>
<template>
  <div class="app-shell">
    <header class="site-header"><nav class="navigation container" aria-label="Main navigation">
      <RouterLink class="brand" to="/">Vue<span>Nav</span></RouterLink>
      <div class="nav-links"><RouterLink class="nav-link" to="/">Home</RouterLink><RouterLink class="nav-link" to="/about">About</RouterLink></div>
    </nav></header>
    <main class="container page-content"><RouterView /></main>
    <footer class="site-footer"><p>Built with Vue 3 · Simple navigation, thoughtfully designed.</p></footer>
  </div>
</template>
