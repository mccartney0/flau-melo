
<script setup lang="ts">
  import ButtonHighlight from './ButtonHighlight.vue';
</script>

<template>
  <div class="wrapper-meet-your-profile">
    <div class="image-container">
      <img src="@/assets/meet-your-profile.png" alt="Flau Melo">
    </div>

    <div class="content-container p-20">
      <div class="title">
        Quer conhecer seu Perfil Comportamental?
      </div>

      <div class="content my-10">
        O DISC Plus é uma excelente opção! Com ele você adquire muito
        autoconhecimento, passa a entender seu potencial em amplitude
        e seus gaps, tendo aí uma base significativa para iniciar seu
        processo de desenvolvimento pessoal e/ou profissional.
      </div>

      <ButtonHighlight
        buttonLabel="FALE COM ESPECIALISTA"
        link="https://api.whatsapp.com/send?phone=556699529479&text=Ol%C3%A1%2C%20gostaria%20de%20conhecer%20um%20pouco%20mais%20sobre%20os%20treinamentos."
        target="_blank"
      />
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .wrapper-meet-your-profile {
    margin-top: 250px;
    width: 100%;
    background-color: var(--vt-c-white-mute);

    .image-container {
      position: relative;

      img {
        position: absolute;
        right: 10%;
        top: -100px;

        width: 500px;
      }
    }

    .content-container {
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
</style>
