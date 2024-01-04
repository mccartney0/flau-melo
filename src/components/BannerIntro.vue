<template>
  <div class="wrapper-banner-intro">
    <div class="banner"></div>
  </div>
</template>

<style lang="scss" scoped>
  .wrapper-banner-intro {
    position: relative;
    height: calc(100vh - var(--navigation-height));
    top: -96px;
    z-index: -1;

    .banner {
      background-image: url('@/assets/bg.png');
      background-position: center;
      background-repeat: no-repeat;
      background-size: cover;
      height: 100vh;
      width: 100%;
    }
  }
</style>
