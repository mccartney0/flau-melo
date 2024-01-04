<script setup lang="ts">
defineProps<{
  link: string,
  buttonLabel: string,
}>()
</script>

<template>
  <a
    :href="link"
    class="wrapper-button-highlight button-highlight p-3 rounded-lg"
  >
    {{ buttonLabel }}
  </a>
</template>

<style lang="scss" scoped>
  .button-highlight {
    background-color: var(--vt-c-white);
    text-align: center;

    &:hover {
      color: var(--vt-c-white);
      background-color: var(--vt-c-white-mute);

      animation: shake 0.82s cubic-bezier(.36,.07,.19,.97) both;
      transform: translate3d(0, 0, 0);
      perspective: 1000px;
    }

    @keyframes shake {
      10%, 100% {
        transform: translate3d(-1px, 0, 0);
      }
      20%, 80% {
        transform: translate3d(1px, 0, 0);
      }
      50%, 70% {
        transform: translate3d(-1px, 0, 0);
      }
      40%, 60% {
        transform: translate3d(1px, 0, 0);
      }
    }
  }
</style>