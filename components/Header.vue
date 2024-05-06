<script setup lang="ts">
const nuxtApp = useNuxtApp();
const { activeHeadings, updateHeadings } = useScrollspy();

const links = computed(() => [
  {
    label: 'Oferta',
    to: '#oferta',
    icon: 'i-heroicons-document-duplicate',
    active: activeHeadings.value.includes('oferta'),
  },
  {
    label: 'Kontakt',
    to: '#kontakt',
    icon: 'i-heroicons-phone',
    active: activeHeadings.value.includes('kontakt'),
  },
  {
    label: 'Pytania i odpowiedzi',
    to: '#faq',
    icon: 'i-heroicons-question-mark-circle',
    active: activeHeadings.value.includes('faq'),
  },
]);

nuxtApp.hooks.hookOnce('page:finish', () => {
  updateHeadings([
    document.querySelector('#oferta'),
    document.querySelector('#kontakt'),
    document.querySelector('#faq'),
  ]);
});
</script>

<template>
  <UHeader :links="links">
    <template #logo>
      Magdalena Garus<UBadge
        label="PERFEKT"
        variant="subtle"
        class="mb-0.5 hidden md:block"
      />
    </template>

    <template #panel>
      <UAsideLinks :links="links" />
    </template>

    <template #right>
      <UColorModeToggle aria-label="Change Color" />
    </template>
  </UHeader>
</template>
