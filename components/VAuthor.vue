<template>
  <dl class="VAuthor">
    <dt class="VAuthor__name">{{ name }}</dt>
    <dd class="VAuthor__title">{{ title }}</dd>
  </dl>
</template>

<script lang="ts" setup>
defineProps<{
  name: string;
  title: string;
}>();
</script>

<style lang="scss">
.VAuthor {
  margin: 0;

  &__name {
    display: block;
    line-height: 1.4;
    font-family: 'Source Sans Pro', sans-serif;
    font-weight: 700;
    font-size: 1.5rem;
    color: #383838;
  }

  &__title {
    display: block;
    margin: 0;
    line-height: 1.4;
    font-family: 'Zilla Slab', sans-serif;
    font-weight: 600;
    font-size: 1.5rem;
    color: #646464;
  }
}
</style>
