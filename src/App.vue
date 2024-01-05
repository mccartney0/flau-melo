<script setup lang="ts">
  import { RouterView } from 'vue-router'
  import HeaderMenu from './components/HeaderMenu.vue';
</script>

<template>
  <div class="app-container">
    <HeaderMenu />
    
    <div class="router-container">
      <RouterView />
    </div>

    <footer>
      Footer
    </footer>
  </div>
</template>

<style scoped>
  @media (min-width: 1400px) {
    .app-container {
      display: flex;
      flex-direction: column;
      align-items: center;
    }

    .router-container {
      width: 1400px;
    }
  }
</style>