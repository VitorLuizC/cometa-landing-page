<template>
  <VSection class="The4thSection">
    <img
      class="The4thSection__figure"
      src="~/assets/images/green-semicircle.svg"
      alt=""
    />

    <VSubtitle class="The4thSection__title">Quer fazer parte?</VSubtitle>

    <p class="The4thSection__text">
      Seja uma das primeiras pessoas a indicar interesse, e avisaremos quando a
      plataforma estiver pronta!
    </p>

    <VButtonLink class="The4thSection__button">Indicar interesse</VButtonLink>
  </VSection>
</template>

<style lang="scss">
.The4thSection {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 4.375rem 4.375rem 5rem;
  background-color: #f5f9ff;

  &__figure {
    margin-bottom: 1.9375rem;
  }

  &__text {
    width: 35.375rem;
    margin: 0;
    margin-bottom: 1.6875rem;
    line-height: 1.4;
    text-align: center;
    font-family: 'Zilla Slab', serif;
    font-weight: 600;
    font-size: 2rem;
    color: #646464;
  }
}
</style>
