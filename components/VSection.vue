<template>
  <section class="VSection">
    <slot></slot>
  </section>
</template>

<style lang="scss">
.VSection {
  grid-column: span 4;

  @media screen and (min-width: 768px) {
    grid-column: span 12;
  }
}
</style>
