<template>
  <h1 class="VTitle">
    <slot></slot>
  </h1>
</template>

<style lang="scss">
@import '../styles/responsive-property.scss';

.VTitle {
  @include responsive-property(font-size, (
    0: 2.3rem,
    640px: 3rem,
    1280px: 4.5rem,
  ));

  margin: 0;
  line-height: 1.2;
  font-family: 'Source Sans Pro', sans-serif;
  font-weight: 700;
  color: #383838;
}
</style>
