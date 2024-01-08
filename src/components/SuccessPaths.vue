<script setup lang="ts">
  import { ref } from 'vue';
  import AccordionItem from './AccordionItem.vue';

  const products = ref([
    {
      id: 1,
      label: 'Life Coaching incluso um emotional intelligence',
      content: 'Trabalha qualquer meta pessoal que você estabeleça. Caso não tenha uma, temos técnicas eficientes para te ajudar a encontrar. Alguns dos benefícios: quebra de crenças limitantes, criação de crenças fortalecedoras, mudança comportamental significativa, melhora na comunicação, produtividade, gestão das emoções e qualidade de vida.'
    },
    {
      id: 2,
      label: 'Relatório Emotional Intelligence + Devolutiva',
      content: 'O Relatório mais utilizado pelas grades empresas e pessoal pós Covid! Uma ferramenta indispensável para as pessoas que desejam entender as próprias competências relacionadas à inteligência emocional.'
    },
    {
      id: 3,
      label: 'Relatório Comportamental DISC Plus + Devolutiva',
      content: 'O DISC Plus é uma excelente opção! Com ele você adquire muito autoconhecimento, passa a entender seu potencial em amplitude e seus gaps, tendo aí uma base significativa para iniciar seu processo de desenvolvimento pessoal e/ou profissional.'
    },
    {
      id: 4,
      label: 'DISC Seleção + Treinamento Coletivo (Colaboradores)',
      content: 'Recrutamento e seleção mais eficientes! Uma poderosa ferramenta para se ter na hora da contratação ou para  avaliar colaboradores para se saber qual ocomportamento deles quando submetidos à situações específicas. O DISC Seleção destaca as características comportamentais das pessoas como forças, motivações , '
    },
    {
      id: 5,
      label: 'Treinamento Executivo (a partir de 15 Sessões)',
      content: 'O treinamento executivo oferece um programa bem completo de desenvolvimento para o profissional que quer Performar. Fazendo uma reprogramação mental personalizada voltada para seus propósitos de ascensão. Reposicionamento profissional, com a ajuda da:  Aromaterapia, Neurociência, Mindfulness e Psicologia Positiva;'
    },
  ])
</script>

<template>
  <div class="wrapper-success-paths gap-20 flex justify-around">
    <img class="flaudiene-image-2" src="@/assets/flaudiene-corpo-inteiro-2.png" alt="">

    <div class="success-paths-container">
      <div class="square-container">
        <img class="two-squares" src="@/assets/two-square.svg" alt="Squares">
      </div>

      <div class="title-container mb-28">
        Caminhos para o Sucesso
      </div>

      <AccordionItem
        v-for="product in products"
        :key="product.id"
        :id="product.id"
        :label="product.label"
        :content="product.content"
      />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.wrapper-success-paths {
  margin-top: 290px;

  .flaudiene-image-2 {
    height: max-content;
  }

  .success-paths-container {
    position: relative;
    
    .square-container {
      position: absolute;
      top: -130px;
      right: 0;
    }

    .title-container {
      color: var(--vt-c-black-soft);
      font-size: 3rem;
      font-weight: 500;
      
    }
  }
}

@media (min-width: 1400px) {
  .wrapper-success-paths {
    .success-paths-container {
      .square-container {
        right: -90px;
      }
    }
  }
}
</style>
