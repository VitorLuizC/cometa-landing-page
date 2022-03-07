<template>
  <h1 class="VTitle">
    <slot></slot>
  </h1>
</template>

<style lang="scss">
.VTitle {
  margin: 0;
  line-height: 1.2;
  font-family: 'Source Sans Pro', sans-serif;
  font-weight: 700;
  font-size: 2.25rem;
  color: #383838;

  @media screen and (max-width: 640px) {
    font-size: 3rem;
  }

  @media screen and (max-width: 1280px) {
    font-size: 4.5rem;
  }
}
</style>
