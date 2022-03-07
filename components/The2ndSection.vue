<template>
  <VSection class="The2ndSection">
    <VSubtitle class="The2ndSection__title">
      Conheça nossas soluções
    </VSubtitle>

    <VCard
      :image="book"
      class="The2ndSection__card"
      title="Conteúdos que se complementam"
      description="Crie conteúdos que outras pessoas podem complementar com o que conhecem"
    />

    <VCard
      :image="pen"
      class="The2ndSection__card"
      title="Projetos evoluídos com feedbacks"
      description="Adicione seus projetos e aprenda com outras pessoas por meio dos feedbacks assertivos"
    />

    <VCard
      :image="dialog"
      class="The2ndSection__card"
      title="Discussões de design"
      description="Converse sobre design de forma ampla, ensine e aprenda com segmentos diferentes"
    />
  </VSection>
</template>

<script lang="ts" setup>
import pen from '~/assets/images/pen.svg';
import book from '~/assets/images/book.svg';
import dialog from '~/assets/images/dialog.svg';
</script>

<style lang="scss">
@import '../styles/responsive-properties.scss';
@import '../styles/responsive-property.scss';

.The2ndSection {
  @include responsive-properties((
    padding-top: (
      0: 4rem,
      640px: 5.3125rem,
    ),
    padding-bottom: (
      0: 4.75rem,
      640px: 6.375rem,
    ),
  ));

  row-gap: 2.25rem;
  background-color: #f5f9ff;

  &__title {
    @include responsive-properties((
      margin-bottom: (
        /* 0: 1.75rem, */
        640px: 3.25rem,
      ),
      text-align: (
        0: center,
        1280px: left,
      ),
    ));

    grid-column: 1 / -1;
  }

  &__card {
    @include responsive-property(grid-column, (
      0: #{'1 / -1'},
      640px: #{'2 / 6'},
      768px: #{'3 / 11'},
      1280px: #{'span 4'},
    ));
  }
}
</style>
