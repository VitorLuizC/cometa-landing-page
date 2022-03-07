<template>
  <VSection class="The1stSection">
    <img class="The1stSection__figure" src="~/assets/images/hands.svg" alt="" />

    <article class="The1stSection__content">
      <VLogo class="The1stSection__logo" />

      <VTitle class="The1stSection__title">Rompa com os silos do design</VTitle>

      <VDescription class="The1stSection__description" large>
        Faça parte da comunidade open-source que tornará o Design mais
        integrado, embasado e estratégico
      </VDescription>

      <VButtonLink>Indicar interesse</VButtonLink>
    </article>
  </VSection>
</template>

<style lang="scss">
.The1stSection {
  display: flex;
  align-items: flex-start;
  justify-content: space-evenly;
  padding-top: calc(var(--logo-height) + 7.0625rem);
  padding-bottom: 8rem;

  & &__logo {
    position: absolute;
    top: calc((var(--logo-height) + 2rem) * -1);
    height: var(--logo-height);
  }

  &__figure {
    // It's an image, so I can't avoid using px
    width: 203px;
  }

  &__content {
    position: relative;
    max-width: 39.25rem;
  }

  &__title {
    margin-bottom: 1.3125rem;
  }

  &__description {
    margin-bottom: 1.3125rem;
  }
}
</style>
