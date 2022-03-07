<template>
  <h2 class="VSubtitle">
    <slot></slot>
  </h2>
</template>

<style lang="scss">
@import '../styles/responsive-property.scss';

.VSubtitle {
  @include responsive-property(font-size, (
    0: 1.5rem,
    640px: 2.75rem,
  ));

  margin: 0;
  line-height: 1.4;
  font-family: 'Source Sans Pro', sans-serif;
  font-weight: 700;
  color: #383838;
}
</style>
