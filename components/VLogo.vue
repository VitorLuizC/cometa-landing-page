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
:root {
  --logo-height: 48px;

  @media screen and (min-width: 768px) {
    --logo-height: 64px;
  }
}

.VLogo {
  display: flex;
  align-items: center;
  height: var(--logo-height);
  margin: 0;

  &__iconographic {
    width: 45.9px;
    height: var(--logo-height);

    @media screen and (min-width: 768px) {
      width: 59.97px;
    }

    @media screen and (min-width: 1366px) {
      width: 64px;
    }
  }

  &__typographic {
    width: 120.25px;
    height: 26.91px;
    margin-left: 14.85px;

    @media screen and (min-width: 768px) {
      width: 157.12px;
      height: 35.88px;
      margin-left: 19.4px;
    }

    @media screen and (min-width: 1366px) {
      width: 167.67px;
      height: 35.88px;
      margin-left: 20.71px;
    }
  }
}
</style>
