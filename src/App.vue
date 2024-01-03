<script setup lang="ts">
import { RouterView } from 'vue-router'
import BannerIntro from './components/BannerIntro.vue';
</script>

<template>
  <BannerIntro />

  <main>
    <RouterView />
  </main>

  <footer>
    Footer
  </footer>
</template>