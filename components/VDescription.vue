<template>
  <p :class="['VDescription', { 'VDescription--large': large }]">
    <slot></slot>
  </p>
</template>

<script lang="ts" setup>
defineProps<{
  large?: boolean;
}>();
</script>

<style lang="scss">
.VDescription {
  margin: 0;
  line-height: 1.4;
  font-family: 'Zilla Slab', serif;
  font-weight: 600;
  font-size: 1.25rem;
  color: #646464;

  @media screen and (min-width: 640px) {
    font-size: 1.5rem;
  }

  &--large {
    @media screen and (min-width: 1280px) {
      font-size: 2rem;
    }
  }
}
</style>
