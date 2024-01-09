<script setup lang="ts">
import { ref } from 'vue';

defineProps<{
  id: number,
  label: string,
  content: string,
}>()

const openTab = ref(1);

const toggleTab = (tab: number) => {
  openTab.value = openTab.value === tab ? 0 : tab;
};

const setTabActive = (tab: number) => {
  return openTab.value === tab ? 'active-tab' : '';
}
</script>

<template>
  <div class="accordion-item">
    <label
      @click="toggleTab(id)"
      :class="['accordion-label cursor-pointer flex items-center p-2',
        setTabActive(id),
      ]">
      <span class="mr-3">
        {{ label }}
      </span>

      <span v-show="openTab === id" class="accordion-icon">
        <i class="bi bi-chevron-up"></i>
      </span>
      <span v-show="openTab !== id" class="accordion-icon">
        <i class="bi bi-chevron-down"></i>
      </span>
    </label>

    <transition name="slide-fade">
      <div v-show="openTab === id" class="accordion-content p-2 mb-5">
        {{ content }}
      </div>
    </transition>
  </div>
</template>

<style lang="scss" scoped>
  .accordion-item {
      width: 600px;
    .accordion-label {
      color: var(--vt-c-black-soft);
      font-size: 1.2rem;
      font-weight: 600;
      border-radius: 6px;

      &:hover {
        background-color: var(--vt-c-white-mute);
      }

      &.active-tab {
        background-color: var(--vt-c-white-mute);
      }
    }
    
    .accordion-content {
      border-bottom: 1px solid var(--vt-c-white-mute);
      color: var(--vt-c-indigo);
      font-size: .95rem;
      font-weight: 400;
    }

    .slide-fade-leave-active,
    .slide-fade-enter-active {
      transition: opacity 0.5s, transform 0.5s;
    }

    .slide-fade-enter,
    .slide-fade-leave-to {
      opacity: 0;
      transform: translateY(20px);
    }
  }

  @media (max-width: 1024px) {
    .accordion-item {
      width: 90%;

      .accordion-label,
      .accordion-content {
        text-align: center;
      }
    }
  }
</style>