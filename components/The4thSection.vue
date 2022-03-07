<template>
  <VSection class="The4thSection">
    <img
      class="The4thSection__figure"
      src="~/assets/images/green-semicircle.svg"
      alt=""
    />

    <VSubtitle class="The4thSection__title">Quer fazer parte?</VSubtitle>

    <VDescription class="The4thSection__text" large>
      Seja uma das primeiras pessoas a indicar interesse, e avisaremos quando a
      plataforma estiver pronta!
    </VDescription>

    <VButtonLink class="The4thSection__button">Indicar interesse</VButtonLink>
  </VSection>
</template>

<style lang="scss">
@import '../styles/responsive-properties.scss';
@import '../styles/responsive-property.scss';

.The4thSection {
  align-content: center;
  padding-top: 4.375rem;
  padding-bottom: 5rem;
  background-color: #f5f9ff;

  &__figure {
    @include responsive-properties((
      grid-column: (
        0: #{'2 / 4'},
        640px: #{'3 / 5'},
        768px: #{'6 / 8'},
      ),
      margin-bottom: (
        0: 1.9375rem,
      ),
    ));
  }

  &__figure,
  &__button {
    margin-left: auto;
    margin-right: auto;
  }

  &__text,
  &__title {
    text-align: center;
  }

  &__title {
    @include responsive-properties((
      grid-column: (
        0: #{'1 / -1'},
        768px: #{'3 / 11'},
        1280px: #{'5 / 9'},
      ),
      margin-bottom: (
        0: 0.125rem,
      ),
    ));
  }

  &__text {
    @include responsive-properties((
      grid-column: (
        0: #{'1 / -1'},
        768px: #{'2 / 12'},
        1280px: #{'4 / 10'},
      ),
      margin-bottom: (
        0: 2.25rem,
        640px: 1.6875rem,
      ),
    ));

    @media screen and (min-width: 640px) {
      font-size: 2rem;
    }
  }

  &__button {
    @include responsive-property(grid-column, (
      0: #{'1 / -1'},
      640px: #{'2 / 6'},
      768px: #{'4 / 10'},
      1280px: #{'5 / 9'},
    ));
  }
}
</style>
