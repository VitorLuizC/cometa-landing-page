<template>
  <VSection class="The1stSection">
    <article class="The1stSection__content">
      <VLogo class="The1stSection__logo" />

      <VTitle class="The1stSection__title">
        Rompa com os silos
        <br />
        do design
      </VTitle>

      <VDescription class="The1stSection__description" large>
        Faça parte da comunidade open-source que tornará o Design mais
        integrado, embasado e estratégico
      </VDescription>

      <VButtonLink>Indicar interesse</VButtonLink>
    </article>

    <figure class="The1stSection__figure">
      <img
        class="The1stSection__image"
        src="~/assets/images/hands.svg"
        alt=""
      />
    </figure>
  </VSection>
</template>

<style lang="scss">
@import '../styles/responsive-properties.scss';
@import '../styles/responsive-property.scss';

.The1stSection {
  @include responsive-properties((
    min-height: (
      768px: 100vh,
    ),
    padding-top: (
      0: 3.875rem,
      640px: 3.75rem,
      768px: 2rem,
    ),
    padding-bottom: (
      0: 3.875rem,
      640px: 2.5rem,
      768px: 2rem,
    ),
  ));

  align-items: center;

  &__content {
    @include responsive-properties((
      margin-bottom: (
        0: 3.5rem,
        768px: 0,
      ),
      grid-column: (
        0: #{'1 / -1'},
        640px: #{'2 / 6'},
        768px: #{'5 / -1'},
        1024px: #{'5 / 11'},
        1280px: #{'5 / 12'},
      ),
      align-items: (
        0: center,
        768px: flex-start,
      ),
    ));

    display: flex;
    flex-direction: column;
  }

  &__figure {
    @include responsive-properties((
      grid-column: (
        0: #{'1 / -1'},
        768px: #{'span 3'},
      ),
      order: (768px: -1),
    ));

    display: flex;
    margin: 0;
    justify-content: center;
  }

  &__image {
    @include responsive-property(max-width, (
      0: 111px,
      768px: 150px,
      1280px: 203px,
    ));

    display: block;
    width: 100%;
  }

  &__logo {
    margin-bottom: 1.875rem;
  }

  &__title {
    @include responsive-properties((
      margin-bottom: (
        0: 0.375rem,
        1280px: 1.25rem,
      ),
      text-align: (
        0: center,
        768px: left,
      ),
    ));
  }

  &__description {
    @include responsive-properties((
      padding: (
        0: 0 0.75rem,
        640px: 0,
      ),
      margin-bottom: (
        0: 2.125rem,
        640px: 3rem,
        1280px: 2.75rem,
      ),
      text-align: (
        0: center,
        768px: left,
      ),
    ));
  }
}
</style>
