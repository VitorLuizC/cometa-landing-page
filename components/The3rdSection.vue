<template>
  <section class="The3rdSection">
    <aside class="The3rdSection__side"></aside>

    <div class="The3rdSection__container">
      <VTitle class="The3rdSection__title">Quais os benefícios em fazer parte?</VTitle>

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
  </section>
</template>

<style lang="scss">
.The3rdSection {
  display: flex;
  align-items: stretch;
  justify-content: space-between;
  background-color: #FFFFFF;

  &__side {
    // It's an image, so I can't avoid using px
    width: 381px;
    padding-bottom: 2px;
    background-clip: content-box;
    background-image: url(~/assets/images/pattern.svg);
    background-repeat: repeat-y;
  }

  &__container {
    width: fit-content;
    margin: 7.8125rem 5.8125rem 7.0625rem 0;
    padding: 2.9375rem;
    border: 1px solid #0066FF;
    border-radius: 1.5625rem;
  }

  &__title {
    margin-bottom: 2.9375rem;
  }

  &__topics {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  &__topic {
    position: relative;
    max-width: 38.75rem;
    margin: 0;
    margin-left: 2.5rem;
    line-height: 1.4;
    font-family: 'Source Sans Pro', sans-serif;
    font-weight: 600;
    font-size: 1.875rem;
    color: #646464;
  }

  &__topic + &__topic {
    margin-top: 2.9375rem;
  }

  &__topic::before {
    position: absolute;
    left: -2.5rem;
    line-height: 1.4;
    font-family: 'Source Sans Pro', sans-serif;
    font-weight: 600;
    font-size: 1.875rem;
    color: #0066FF;
    content: '•';
  }
}
</style>
