
<script setup lang="ts">
  import ButtonHighlight from './ButtonHighlight.vue';
</script>

<template>
  <div class="wrapper-banner-intro">
    <div class="banner flex justify-around items-center">
      <img class="background-image" src="@/assets/bg.png" alt="Flau Melo, Background">

      <div class="banner-container">
        <div class="banner-message mb-10 text-2xl">
          Nosso objetivo é guiá-lo(a) na jornada
          de transformação, capacitando-o(a)
          a superar desafios, estabelecer metas significativas e alcançar
          o sucesso em todas as áreas da vida.
        </div>

        <ButtonHighlight
          link="#mentorias"
          buttonLabel="Conheça o que oferecemos"
          target="_self"
        />
      </div>

      <div class="image-container mt-28">
        <img class="flaudiene-image" src="@/assets/flau-melo.png" alt="Flau Melo">
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
        height: 900px;
        width: 100%;
        z-index: -1;
      }

      .banner-message {
        width: 460px;
        color: var(--vt-c-black-soft);
        font-weight: 600;
      }

    }

    @media (max-width: 767px) {
      .banner {
        flex-direction: column;

        .banner-container {
          margin-top: 70px;
          margin-bottom: -60px;
          display: flex;
          flex-direction: column;
          justify-content: center;
          align-items: center;

          .banner-message {
            width: 100vw;
            font-size: 1.2rem;
            text-align: center;
          }
        }
      }

      .image-container {
        .flaudiene-image {
          height: 350px;
        }
      }
    }
  }
</style>
