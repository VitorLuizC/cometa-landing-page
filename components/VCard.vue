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
.VCard {
  width: 100%;
  max-width: 23.125rem;
  padding: 2.625rem 3.65625rem;
  background-color: #ffffff;
  border: 1px solid #a8cbff;
  border-radius: 1.5625rem;

  &__image {
    display: block;
    width: auto;
    max-width: 8.8125rem;
    height: 9.125rem;
    margin-bottom: 1.5625rem;
    object-fit: scale-down;
  }

  &__title {
    margin: 0;
    line-height: 1.4;
    font-family: 'Source Sans Pro', sans-serif;
    font-weight: 700;
    font-size: 1.875rem;
    color: #383838;
  }
}
</style>
