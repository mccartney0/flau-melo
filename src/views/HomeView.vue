<script setup lang="ts">
  import About from '@/components/About.vue';
  import BannerIntro from '@/components/BannerIntro.vue';
  import CompanyHighlights from '@/components/CompanyHighlights.vue';
  import Contact from '@/components/Contact.vue';
  import MeetYourProfile from '@/components/MeetYourProfile.vue';
  import SuccessPaths from '@/components/SuccessPaths.vue';
</script>

<template>
  <div class="home">
    <BannerIntro id="home" />
    <CompanyHighlights />
    <SuccessPaths id="mentorias" />
    <MeetYourProfile />
    <About id="sobre" />
    <Contact />
  </div>
</template>

