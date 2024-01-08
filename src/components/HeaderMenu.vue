
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
        <a href="#" class="nav-link">Home</a>
        <a href="#mentorias" class="nav-link">Mentorias</a>
        <a href="#clientes" class="nav-link">Clientes</a>
        <a href="#sobre" class="nav-link">Sobre</a>
        <ButtonHighlight
          buttonLabel="FALE COM ESPECIALISTA"
          link="https://api.whatsapp.com/send?phone=556699529479&text=Ol%C3%A1%2C%20gostaria%20de%20conhecer%20um%20pouco%20mais%20sobre%20os%20treinamentos."
          target="_blank"
        />
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