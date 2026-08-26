<script setup>
import { ref, computed } from 'vue'
import HomeView from './views/HomeView.vue'
import AboutView from './views/AboutView.vue'

const currentPage = ref('home')
const pages = { home: HomeView, about: AboutView }
const activePage = computed(() => pages[currentPage.value])

function navigate(page) {
  currentPage.value = page
}
</script>

<template>
  <div class="app-shell">
    <header class="site-header"><nav class="navigation container" aria-label="Main navigation">
      <button class="brand" type="button" @click="navigate('home')">Vue<span>Nav</span></button>
      <div class="nav-links"><button class="nav-link" :class="{ 'router-link-active': currentPage === 'home' }" type="button" @click="navigate('home')">Home</button><button class="nav-link" :class="{ 'router-link-active': currentPage === 'about' }" type="button" @click="navigate('about')">About</button></div>
    </nav></header>
    <main class="container page-content"><component :is="activePage" @navigate="navigate" /></main>
    <footer class="site-footer"><p>Built with Vue 3 · Simple navigation, thoughtfully designed.</p></footer>
  </div>
</template>
