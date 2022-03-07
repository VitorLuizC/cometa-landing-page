<template>
  <VSection class="The3rdSection">
    <aside class="The3rdSection__side"></aside>

    <div class="The3rdSection__container">
      <VSubtitle class="The3rdSection__title">
        Quais os benefícios em fazer parte?
      </VSubtitle>

      <ul class="The3rdSection__topics">
        <li class="The3rdSection__topic">
          Comunidade <strong>colaborativa e engajada</strong>, onde todas as
          pessoas podem falar e ouvir
        </li>
        <li class="The3rdSection__topic">
          <strong>Pessoas legitimadas</strong> na comunidade de design,
          oferecendo teoria e embasamento
        </li>
        <li class="The3rdSection__topic">
          Pontos de vista distintos alimentados por
          <strong>segmentos diferentes</strong> do design
        </li>
        <li class="The3rdSection__topic">
          <strong>Constante atualização</strong>, podendo rever teorias
          ultrapassadas
        </li>
        <li class="The3rdSection__topic">
          <strong>Diálogo com empatia</strong>, através do nosso guia de
          comunicação na plataforma
        </li>
      </ul>
    </div>
  </VSection>
</template>

<style lang="scss">
@import '../styles/responsive-property.scss';

.The3rdSection {
  padding-top: 4.5rem;
  padding-bottom: 4.5rem;
  background-color: #ffffff;

  &__side {
    @include responsive-property(left, (
      0: -381px,
      768px: calc(5rem - 381px),
      1280px: 0,
    ));

    position: absolute;
    top: 0;
    bottom: 0;

    // It's an image, so I can't avoid using px
    width: 381px;
    padding-bottom: 2px;
    background-clip: content-box;
    background-image: url(~/assets/images/pattern.svg);
    background-repeat: repeat-y;
  }

  &__container {
    @include responsive-property(grid-column, (
      0: #{'1 / -1'},
      1280px: #{'5 / -1'},
    ));

    @include responsive-property(padding, (
      0: 2.5rem,
      640px: 2.9375rem,
    ));

    height: fit-content;
    border: 1px solid #0066ff;
    border-radius: 1.5625rem;
  }

  &__topics {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  &__topic {
    @include responsive-property(font-size, (
      0: 1.25rem,
      640px: 1.5rem,
      1280px: 1.875rem,
    ));

    @include responsive-property(margin, (
      0: 2.5rem 0 0 2.5rem,
      640px: 2.9375rem 0 0 2.5rem,
    ));

    position: relative;
    line-height: 1.4;
    font-family: 'Source Sans Pro', sans-serif;
    font-weight: 600;
    color: #646464;
  }

  &__topic::before {
    position: absolute;
    left: -2.5rem;
    line-height: 1.4;
    font-family: 'Source Sans Pro', sans-serif;
    font-weight: 600;
    font-size: 1.875rem;
    color: #0066ff;
    content: '•';
  }
}
</style>
