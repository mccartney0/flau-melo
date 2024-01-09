
<script setup lang="ts">
  import { ref } from 'vue';
  import ButtonHighlight from '@/components/ButtonHighlight.vue';

  const isWhatsAppButtonActive = ref(false);

  const scrollToSection = (sectionName: string) => {
    const targetElement = document.getElementById(sectionName);
    if (targetElement) {
      targetElement.scrollIntoView({ behavior: 'smooth' });
    }
  }

  const animateWhatsAppButton = (isActive: boolean) => {
    isWhatsAppButtonActive.value = isActive;
  }
</script>

<template>
  <header>
    <nav class="flex items-center justify-evenly pt-4">
      <div class="logo">
        <img src="@/assets/logo.png" alt="Logo">
      </div>

      <div class="links flex items-center justify-evenly">
        <a href="#home" @click.prevent="scrollToSection('home')" class="nav-link">Home</a>
        <a href="#mentorias" @click.prevent="scrollToSection('mentorias')" class="nav-link">Mentorias</a>
        <a href="#clientes" @click.prevent="scrollToSection('clientes')" class="nav-link">Clientes</a>
        <a href="#sobre" @click.prevent="scrollToSection('sobre')" class="nav-link">Sobre</a>
        <ButtonHighlight
          buttonLabel="FALE COM ESPECIALISTA"
          link="https://api.whatsapp.com/send?phone=556699529479&text=Ol%C3%A1%2C%20gostaria%20de%20conhecer%20um%20pouco%20mais%20sobre%20os%20treinamentos."
          target="_blank"
        />
      </div>
    </nav>

    <a
      class="whats-app-button flex justify-center items-center"
      @mouseover="() => animateWhatsAppButton(true)"
      @mouseout="() => animateWhatsAppButton(false)"
      href="https://api.whatsapp.com/send?phone=556699529479&text=Ol%C3%A1%2C%20gostaria%20de%20conhecer%20um%20pouco%20mais%20sobre%20os%20treinamentos."
      target="_blank"
    >
      <i class="bi bi-whatsapp" style="font-size: 1.7rem"></i>
    </a>
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

  .whats-app-button {
    cursor: pointer;
    position: fixed;
    background-color: #28D230;
    color: var(--vt-c-white);
    width: 50px;
    height: 50px;
    border-radius: 50%;

    right: 20px;
    bottom: 20px;

    transition: transform 0.3s ease;
    z-index: 99;

    &:hover {
      transform: scale(1.2);
    }
  }

  @media (min-width: 1400px) {
    nav {
      width: 1400px;
    }
  }
</style>