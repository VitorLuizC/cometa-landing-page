<template>
  <section class="VSection">
    <slot></slot>
  </section>
</template>

<style lang="scss">
.VSection {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  column-gap: 1rem;

  @media screen and (min-width: 640px) {
    column-gap: 1.25rem;
  }

  @media screen and (min-width: 768px) {
    grid-template-columns: repeat(12, 1fr);
  }
}
</style>
