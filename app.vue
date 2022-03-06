<template>
  <Link rel="preconnect" href="https://fonts.googleapis.com" />

  <Link
    rel="preconnect"
    href="https://fonts.gstatic.com"
    crossorigin="crossorigin"
  />

  <Link
    rel="stylesheet"
    href="https://fonts.googleapis.com/css2?family=Source+Sans+Pro:wght@600;700&family=Zilla+Slab:wght@600&display=swap"
  />

  <Link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png" />

  <Link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png" />

  <Link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png" />

  <Link rel="manifest" href="/site.webmanifest" />

  <Link rel="mask-icon" href="/safari-pinned-tab.svg" color="#5bbad5" />

  <Meta name="apple-mobile-web-app-title" content="Cometa" />

  <Meta name="application-name" content="Cometa" />

  <Meta name="msapplication-TileColor" content="#da532c" />

  <Meta name="theme-color" content="#ffffff" />

  <!-- Open Graph / Facebook -->

  <Meta property="og:type" content="website" />

  <Meta property="og:url" :content="url" />

  <Meta property="og:title" :content="title" />

  <Meta property="og:description" :content="description" />

  <Meta property="og:image" :content="preview" />

  <!-- Twitter -->

  <Meta property="twitter:card" content="summary_large_image" />

  <Meta property="twitter:url" :content="url" />

  <Meta property="twitter:title" :content="title" />

  <Meta property="twitter:description" :content="description" />

  <Meta property="twitter:image" :content="preview" />

  <Title>{{ title }}</Title>

  <Meta name="title" :content="title" />

  <Meta name="description" :content="description" />

  <Meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <main class="App">
    <The1stSection />
    <The2ndSection />
    <The3rdSection />
    <The4thSection />
  </main>

  <TheFooter />
</template>

<script lang="ts" setup>
import preview from '~/assets/images/preview.png';

const url = 'https://cometa-landing-page.vercel.app/';
const title = 'Cometa - Rompa com os silos do design';
const description =
  'Faça parte da comunidade open-source que tornará o Design mais integrado, embasado e estratégico';
</script>

<style lang="scss">
*,
*::before,
*::after {
  box-sizing: border-box;
}

html {
  font-size: 100%;
}

body {
  overflow-x: hidden;
  margin: 0;
}

.App {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  column-gap: 1rem;

  @media screen and (min-width: 640px) {
    column-gap: 1.25rem;
  }

  @media screen and (min-width: 768px) {
    grid-template-columns: repeat(12, 1fr);
  }
}
</style>
