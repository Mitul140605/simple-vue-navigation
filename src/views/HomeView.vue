<script setup>
import { RouterLink } from 'vue-router'
</script>
<template>
  <section class="hero"><div class="hero-copy"><p class="eyebrow">A tiny app with a clear purpose</p><h1>Move around with <span>ease.</span></h1><p class="intro">Welcome to a simple Vue navigation experience. Explore the app and learn how its pieces fit together.</p><RouterLink class="button" to="/about">Learn about this app <span aria-hidden="true">→</span></RouterLink></div><div class="hero-art" aria-hidden="true"><div class="orbit orbit-one"></div><div class="orbit orbit-two"></div><div class="compass">✦</div></div></section>
  <section class="feature-grid" aria-label="Highlights"><article class="feature-card"><span class="feature-icon">01</span><h2>Focused</h2><p>Only the essentials, keeping every interaction straightforward.</p></article><article class="feature-card"><span class="feature-icon">02</span><h2>Responsive</h2><p>A comfortable experience on large screens and small devices.</p></article><article class="feature-card"><span class="feature-icon">03</span><h2>Vue powered</h2><p>Fast, reactive views connected by clean client-side routing.</p></article></section>
</template>
