<template>
  <a
    class="VButtonLink"
    rel="noopener noreferrer"
    href="https://bianca536991.typeform.com/to/P5IzkG6J"
    target="_blank"
    @click.prevent="handleClick"
  >
    <span class="VButtonLink__text">
      <slot></slot>
    </span>
  </a>
</template>

<script lang="ts" setup>
import type { Popup } from '@typeform/embed';

let popup: Popup | null = null;

onMounted(async () => {
  const { createPopup } = await import('@typeform/embed');

  popup = createPopup('P5IzkG6J');
});

const handleClick = () => {
  popup?.open();
};
</script>

<style lang="scss">
@import '@typeform/embed/build/css/popup.css';

.VButtonLink {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  width: fit-content;
  height: fit-content;
  padding: 0.59375rem 2.375rem;
  border-radius: 0.625rem;
  background-color: #0066ff;

  // Reset anchor styles
  text-decoration: none;

  &__text {
    line-height: 1.4;
    font-family: 'Source Sans Pro', sans-serif;
    font-weight: 600;
    font-size: 1.875rem;
    color: #ffffff;
  }
}
</style>
