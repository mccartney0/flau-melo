<script setup lang="ts">
  import { RouterView } from 'vue-router'
  import HeaderMenu from './components/HeaderMenu.vue';
</script>

<template>
  <HeaderMenu />

  <RouterView />

  <footer>
    Footer
  </footer>
</template>