<template>
  <div class="wrapper-about flex justify-evenly gap-10">
    <img src="@/assets/flau-melo-3.png" alt="Flau Melo">

    <div class="about-container">
      <div class="title text-3xl my-8">
        UM POUCO SOBRE MIM
      </div>

      <div class="content text-lg">
        <p>Olá, eu sou Flau Melo.</p>

        <ul>
          <li>Esposa dedicada e mãe apaixonada de dois filhos.</li>
          <li>Ciclista, corredora, praticante de musculação, comprometida com a saúde em todos os aspectos.</li>
          <li>Professora Especialista em:</li>
          <li class="specialization"> • Língua Portuguesa e Literaturas pela UNEMAT/MT, com 13 anos de experiência em sala de aula.</li>
          <li class="specialization"> • Neurociência Psicóloga Positiva Mindfulness pela PUC/PR.</li>
          <li>Fascinada pela mente e pelo comportamento humanos, acredito firmemente que o conhecimento, quando internalizado e combinado com as estratégias certas, transforma vidas.</li>
          <li>Ofereço treinamentos, mentoria, processos de coaching e consultoria empresarial, guiada pela máxima: "<span class="highlight">Nós somos o que fazemos repetidamente. Excelência, portanto, não é um ato, é um hábito!</span>"</li>
        </ul>
        
        <p>Profundamente conectada com a fonte divina.</p>
        <p>Acredito que estamos "mergulhados na mente de Deus."</p>

        <p class="pt-5">Venha transformar sua vida!</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .wrapper-about {
    margin: 220px 0;

    img {
      position: relative;
    }

    .about-container {
      color: var(--vt-c-black-soft);

      .content {
        width: 650px;

        ul {
          padding: 0;

          li {
            margin-bottom: 10px;

            &.specialization {
              font-weight: bold;
              color: #e66150;
            }

            .highlight {
              background-color: var(--vt-c-white-mute);
              padding: 2px;
            }
          }
        }
      }
    }
  }

  @media (max-width: 1024px) {
    .wrapper-about {
      margin: 100px 0;
      display: block;
      img {
        margin: 0 auto;
        height: 350px;
      }
      .about-container {
        text-align: center;
        .content {
          width: 100%;
        }
      }
    }
  }
</style>
