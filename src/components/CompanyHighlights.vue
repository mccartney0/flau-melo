<script setup lang="ts">
</script>

<template>
  <div class="wrapper-company-highlights flex">
    <div class="first-box flex justify-center items-center">
      <div class="box-container">
        <div class="title mb-6">
          <a
            class="contact-link"
            href="https://api.whatsapp.com/send?phone=556699529479&text=Ol%C3%A1%2C%20gostaria%20de%20conhecer%20um%20pouco%20mais%20sobre%20os%20treinamentos."
            target="_blank"
            rel="noopener noreferrer"
          >
            ENTRE EM CONTATO
          </a>
        </div>

        <div class="content">
          NÓS SOMOS AQUILO QUE FAZEMOS
          REPETIDAMENTE. EXCELÊNCIA,
          PORTANTO, NÃO É UM ATO
          MAS SIM UM HÁBITO.
        </div>
      </div>
    </div>

    <div class="second-box flex justify-center items-center">
      <div class="box-container">
        <p>Life Coaching</p>
        <p>Relatório Emotional</p>
        <p>Relatório Comportamental</p>
        <p>Treinamentos</p>

        <div class="content flex justify-center">
          <a
            class="more-button mt-10"
            href="https://api.whatsapp.com/send?phone=556699529479&text=Ol%C3%A1%2C%20gostaria%20de%20saber%20sobre%20seus%20treinamentos."
            target="_blank"
            rel="noopener noreferrer"
          >
            Saiba mais
          </a>
        </div>
      </div>
    </div>

    <div class="third-box flex justify-center items-center">
      <div class="box-container">
        <div class="number-of-customers">
          +352
        </div>

        <div class="title my-2">
          Pessoas impactadas
        </div>

        <div class="content">
          Mentorias, treinamentos executivos e 
          coletivos, sessões de coaching para você e
          seu negócio aqui! Fale conosco.
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .wrapper-company-highlights {
    margin: 0 auto;
    width: 1000px;
    height: 250px;
    background-color: var(--vt-c-white);
    box-shadow: 0px 0px 10px 6px rgba(0, 0, 0, 0.06);

    .first-box,
    .second-box,
    .third-box {
      width: 33.337%;
    }

    .first-box {
      .title {
        .contact-link {
          color: #E57D6F;
          font-weight: 600;
        }
      }

      .content {
        color: var(--vt-c-black-soft);
        width: 260px;
      }
    }

    .second-box {
      background-color: #F8F7F6;

      .content {
        color: var(--vt-c-black-soft);

        .more-button {
          padding: 7px 16px;
          border-radius: 80px;
          background-color: var(--vt-c-white);

          &:hover {
            background-color: var(--vt-c-white-mute);
          }
        }
      }
    }

    .third-box {
      background-color: var(--vt-c-white-mute);

      .number-of-customers {
        font-size: 3rem;
      }

      .title {
        font-size: 1.5rem;
      }

      .content {
        width: 260px;
      }
    }
  }

  @media (min-width: 1400px) {
    .wrapper-company-highlights {
      width: 100%;
      position: relative;
      top: -80px;
      height: 360px;
    }
  }

  @media (max-width: 968px) {
    .wrapper-company-highlights {
      width: 100%;
      height: auto;
      flex-direction: column-reverse;
      justify-content: center;
      align-items: center;

      .first-box,
      .second-box,
      .third-box {
        width: 100%;
        padding: 25px 0;
      }
    }
  }
</style>