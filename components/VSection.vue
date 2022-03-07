<template>
  <section class="VSection">
    <slot></slot>
  </section>
</template>

<style lang="scss">
@import '../styles/responsive-properties.scss';

.VSection {
  @include responsive-properties((
    grid-template-columns: (
      0: repeat(4, 1fr),
      640px: repeat(6, 1fr),
      768px: repeat(12, 1fr),
    ),
    column-gap: (
      0: 1rem,
      640px: 1.25rem,
    ),
    min-height: (768px: 100vh),
    padding-left: (
      0: 2rem,
      768px: 6rem,
    ),
    padding-right: (
      0: 2rem,
      768px: 6rem,
    ),
  ));

  display: grid;
}
</style>
