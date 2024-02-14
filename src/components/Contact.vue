
<script setup lang="ts">
  import ButtonHighlight from './ButtonHighlight.vue';
</script>

<template>
  <div class="wrapper-meet-your-profile">
    <div class="image-container">
      <img src="@/assets/flau-melo-contact.jpeg" alt="Flau Melo">
    </div>

    <div class="content-container p-20">
      <div class="title">
        Nosso Canal de Comunicação
      </div>

      <div class="content my-10 flex flex-col gap-4">
        <div class="whatsapp">
          <a class="flex gap-4 items-center"
            href="https://api.whatsapp.com/send?phone=556699529479&text=Ol%C3%A1%2C%20gostaria%20de%20conhecer%20um%20pouco%20mais%20sobre%20os%20treinamentos."
            target="_blank"
          >
            <img src="@/assets/whatsapp-icon.svg" alt="WhatsApp icon">
            <p>(66) 9.9952-9479</p>
          </a>
        </div>

        <div class="instagram">
          <a class="flex gap-4 items-center" href="https://www.instagram.com/flaudiene_melo" target="_blank">
            <img src="@/assets/instagram-icon.svg" alt="Flau Melo, Instagram icon">
            <p>flaudiene_melo</p>
          </a>
        </div>

        <div class="youtube">
          <a class="flex gap-4 items-center" href="https://www.youtube.com/@FlauMeloCoach" target="_blank">
            <img src="@/assets/youtube-icon.png" alt="Flau Melo, Youtube icon">
            <p>FlauMeloCoach</p>
          </a>
        </div>

        <div class="email">
          <a class="flex gap-4 items-center" href="mailto:treinamento@flaumelo.com.br" target="_blank">
            <i class="bi bi-envelope big" style="font-size: 2rem; color: #4b4b4b;"></i>
            <p>treinamento@flaumelo.com.br</p>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .wrapper-meet-your-profile {
    margin-top: 250px;
    width: 100%;
    background-color: #F3DAC4;;

    .image-container {
      position: relative;

      img {
        position: absolute;
        right: 10%;
        top: -100px;

        width: 350px;
      }
    }

    .content-container {
      color: var(--vt-c-indigo);
      width: 700px;

      .title {
        color: var(--vt-c-black-soft);
        font-size: 3rem;
        font-style: normal;
        font-weight: 400;
        line-height: normal;
      }
    }
  }

  @media (max-width: 1024px) {
    .wrapper-meet-your-profile {
      margin-top: 50px;

      .image-container {
        padding-top: 40px;
        display: flex;
        align-items: center;
        justify-content: center;
        img {
          position: static;
        }
      }
      .content-container {
        padding: 14px;
        padding-bottom: 40px;
        margin-top: 40px;
        width: 100%;
        .title {
          font-size: 2rem;
        }
      }
    }
  }
</style>
