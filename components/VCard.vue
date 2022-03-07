<template>
  <div class="VCard">
    <img class="VCard__image" :src="image" alt="" />
    <h3 class="VCard__title">{{ title }}</h3>
    <VDescription class="VCard__description">{{ description }}</VDescription>
  </div>
</template>

<script lang="ts" setup>
defineProps<{
  image: string;
  title: string;
  description: string;
}>();
</script>

<style lang="scss">
@import '../styles/responsive-property.scss';

.VCard {
  @include responsive-property(padding, (
    0: 1rem 1.875rem,
    640px: 2.625rem 3.65625rem,
  ));

  width: 100%;
  max-width: 23.125rem;
  margin: 0 auto;
  background-color: #ffffff;
  border: 1px solid #a8cbff;
  border-radius: 1.5625rem;

  &__image {
    @include responsive-property(margin, (
      0: 0 auto,
      640px: 0 0 1.5625rem,
    ));

    display: block;
    width: auto;
    max-width: 8.8125rem;
    height: 9.125rem;
    object-fit: scale-down;
  }

  &__title,
  &__description {
    @include responsive-property(text-align, (
      0: center,
      640px: left,
    ));
  }

  &__title {
    @include responsive-property(font-size, (
      0: 1.5rem,
      640px: 1.875rem,
    ));

    margin: 0;
    margin-bottom: 0.75rem;
    line-height: 1.4;
    font-family: 'Source Sans Pro', sans-serif;
    font-weight: 700;
    color: #383838;
  }
}
</style>
