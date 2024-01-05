
<script setup lang="ts">
  import ButtonHighlight from '@/components/ButtonHighlight.vue';
</script>

<template>
  <header>
    <nav class="flex items-center justify-evenly pt-4">
      <div class="logo">
        <img src="@/assets/logo.png" alt="Logo">
      </div>

      <div class="links flex items-center justify-evenly">
        <RouterLink to="/" class="nav-link">Home</RouterLink>
        <RouterLink to="/mentorias" class="nav-link">Mentorias</RouterLink>
        <RouterLink to="/clientes" class="nav-link">Clientes</RouterLink>
        <RouterLink to="/sobre" class="nav-link">Sobre</RouterLink>
        <ButtonHighlight link="/WhatsApp" buttonLabel="FALE COM ESPECIALISTA"/>
      </div>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
  nav {
    .links {
      color: var(--vt-c-black-mute);
      width: 70%;

      .nav-link {
        width: 20px;
        transition: font-size 0.3s ease;

        &:hover {
          font-weight: 600;
          font-size: .97rem;
        }
      }
    }

  }

  @media (min-width: 1400px) {
    nav {
      width: 1400px;
    }
  }
</style>