<template>
  <footer class="TheFooter">
    <VSubtitle class="TheFooter__title">Idealizado por</VSubtitle>

    <VAuthor
      class="TheFooter__author"
      name="Bianca Elias"
      title="Designer de Produto (UX/UI)"
    />

    <VAuthor
      class="TheFooter__author"
      name="Walter Corsi"
      title="Designer de Produto (Físico)"
    />

    <VAuthor
      class="TheFooter__author"
      name="Paulo Lemos"
      title="Designer de Móveis"
    />

    <VAuthor
      class="TheFooter__author"
      name="Matheus Cescon"
      title="Designer Audiovisual"
    />
  </footer>
</template>

<style lang="scss">
@import '../styles/responsive-property.scss';

$border-height: 0.875rem;

.TheFooter {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  row-gap: 1.25rem;
  position: relative;
  padding: 3.125rem;
  padding-top: calc(3.125rem + $border-height);
  border-top: $border-height solid #3cd3b6;
  background-color: #f5f9ff;

  &::before {
    position: absolute;
    top: 0;
    left: 0;
    display: block;
    width: 100%;
    height: $border-height;
    background-color: #ff5e33;
    content: '';
  }

  &__title {
    grid-column: 1 / -1;
  }

  &__author {
    @include responsive-property(grid-column, (
      0: #{'1 / -1'},
      768px: #{'span 2'},
      1280px: #{'span 1'},
    ));
  }
}
</style>
