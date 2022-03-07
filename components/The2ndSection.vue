<template>
  <VSection class="The2ndSection">
    <div class="The2ndSection__content">
      <VSubtitle class="The2ndSection__title">
        Conheça nossas soluções
      </VSubtitle>

      <div class="The2ndSection__cards">
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
      </div>
    </div>
  </VSection>
</template>

<script lang="ts" setup>
import pen from '~/assets/images/pen.svg';
import book from '~/assets/images/book.svg';
import dialog from '~/assets/images/dialog.svg';
</script>

<style lang="scss">
.The2ndSection {
  padding: 5.3125rem 0 6.375rem;
  background-color: #f5f9ff;

  &__content {
    width: fit-content;
    margin: 0 auto;
  }

  &__title {
    margin-bottom: 3.125rem;
  }

  &__cards {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: flex-start;
    gap: 2.25rem;
  }
}
</style>
