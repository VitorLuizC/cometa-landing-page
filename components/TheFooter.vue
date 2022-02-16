<template>
  <footer class="TheFooter">
    <div class="TheFooter__content">
      <VTitle class="TheFooter__title">Idealizado por</VTitle>

      <div class="TheFooter__authors">
        <VAuthor name="Bianca Elias" title="Designer de Produto (UX/UI)" />

        <VAuthor name="Walter Corsi" title="Designer de Produto (Físico)" />

        <VAuthor name="Paulo Lemos" title="Designer de Móveis" />
      </div>
    </div>
  </footer>
</template>

<style lang="scss">
$border-height: 0.875rem;

.TheFooter {
  box-sizing: border-box;
  position: relative;
  width: 100%;
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

  &__content {
    width: fit-content;
    margin: 0 auto;
  }

  &__title {
    margin-bottom: 1.25rem;
  }

  &__authors {
    display: flex;
    flex-wrap: wrap;
    gap: 5.625rem;
    justify-content: space-between;
  }
}
</style>
