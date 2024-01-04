<script setup lang="ts">
  import { RouterView } from 'vue-router'
  import HeaderMenu from './components/HeaderMenu.vue';
</script>

<template>
  <HeaderMenu />

  <main>
    <RouterView />
  </main>

  <footer>
    Footer
  </footer>
</template>

<style lang="scss" scoped>
  main {
    height: calc(100vh - var(--navigation-height));
  }
</style>