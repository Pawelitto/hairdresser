<script setup lang="ts">
useHead({
  meta: [{ name: 'viewport', content: 'width=device-width, initial-scale=1' }],
  link: [{ rel: 'icon', href: '/logo.ico' }],
  htmlAttrs: {
    lang: 'pl',
  },
});

useSeoMeta({
  ogImage: 'https://i.ibb.co/XC9DDZg/banner.jpg',
  twitterImage: 'https://i.ibb.co/XC9DDZg/banner.jpg',
  twitterCard: 'summary_large_image',
  ogUrl: 'https://i.ibb.co/XC9DDZg/banner.jpg',
  twitterTitle: 'Magdalena Garus - Salon Fryzjerski Perfekt',
  twitterDescription: 'Odkryj swoją nową fryzurę już dziś',
});
</script>

<template>
  <Header />

  <UMain>
    <NuxtPage />
  </UMain>

  <Footer />
  <UNotifications />
</template>
