<script setup lang="ts">
  import About from '@/components/About.vue';
  import BannerIntro from '@/components/BannerIntro.vue';
  import CompanyHighlights from '@/components/CompanyHighlights.vue';
  import MeetYourProfile from '@/components/MeetYourProfile.vue';
  import SuccessPaths from '@/components/SuccessPaths.vue';
</script>

<template>
  <div class="home">
    <BannerIntro />
    <CompanyHighlights id="mentorias"/>
    <SuccessPaths />
    <MeetYourProfile />
    <About id="sobre" />
  </div>
</template>

