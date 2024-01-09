<script setup lang="ts">
const currentYear = new Date().getFullYear();
</script>

<template>
  <footer class="flex justify-center flex-col items-center gap-5 p-10">
    <img src="@/assets/logo-black.svg" alt="Flau Melo Logo">
    <p>© {{ currentYear }} Todos os direitos reservados.</p>
  </footer>
</template>


<style lang="scss" scoped>
  footer {
    background-color: var(--vt-c-white-soft);
    width: 100%;

    img {
      width: 106px;
      max-width: 100%;
    }

    p {
      font-weight: 600;
      color: var(--vt-c-black-soft);
    }
  }
</style>