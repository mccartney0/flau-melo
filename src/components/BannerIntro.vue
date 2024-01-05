
<script setup lang="ts">
  import ButtonHighlight from './ButtonHighlight.vue';
</script>

<template>
  <div class="wrapper-banner-intro">
    <div class="banner flex justify-evenly items-center">
      <img class="background-image" src="@/assets/bg.png" alt="Background">

      <div class="mt-6">
        <div class="banner-message mb-10 text-2xl">
          Nosso objetivo é guiá-lo(a) na jornada
          de transformação, capacitando-o(a)
          a superar desafios, estabelecer metas significativas e alcançar
          o sucesso em todas as áreas da vida.
        </div>

        <ButtonHighlight link="#products" buttonLabel="Conheça o que oferecemos" />
      </div>

      <div class="flaudiene-image mt-28">
        <img src="@/assets/flaudiene-corpo-inteiro.png" alt="Flaudiene Melo">
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .wrapper-banner-intro {
    .banner {
      .background-image {
        position: absolute;
        top: 0;
        height: 100vh;
        width: 100%;
        z-index: -1;
      }

      .banner-message {
        width: 460px;
        color: var(--vt-c-black-soft);
        font-weight: 600;
      }
    }
  }
</style>
