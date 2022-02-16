<template>
  <a class="VButtonLink" href="#">
    <span class="VButtonLink__text">
      <slot></slot>
    </span>
  </a>
</template>

<style lang="scss">
.VButtonLink {
  display: inline-flex;
  align-items: center;
  justify-content: center;
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
