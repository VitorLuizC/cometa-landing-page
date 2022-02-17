<template>
  <figure class="VLogo">
    <img
      class="VLogo__iconographic"
      src="~/assets/images/iconographic-logo.svg"
      alt=""
    />
    <img
      class="VLogo__typographic"
      src="~/assets/images/typographic-logo.svg"
      alt="Cometa"
    />
  </figure>
</template>

<style lang="scss">
.VLogo {
  display: flex;
  align-items: center;
  height: 4rem;
  margin: 0;

  &__typographic {
    margin-left: 1.25rem;
  }
}
</style>
