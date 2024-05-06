<script setup lang="ts">
const links = [
  {
    label: "Resources",
    to: "/resources",
  },
  {
    label: "Features",
    to: "/features",
  },
  {
    label: "Company",
    to: "/company",
  },
];

const toast = useToast();

const email = ref("");
const loading = ref(false);

function onSubmit() {
  loading.value = true;

  setTimeout(() => {
    toast.add({
      title: "Subscribed!",
      description: "You've been subscribed to our newsletter.",
    });

    loading.value = false;
  }, 1000);
}
</script>

<template>
  <UFooter>
    <template #left>
      <NuxtLink
        to="https://github.com/Pawelitto"
        target="_blank"
        class="flex items-center"
      >
        <p>Stworzone przez:&nbsp;</p>
        <span class="text-primary-500 dark:text-primary-400 font-bold">
          Paweł Pietras</span
        >
      </NuxtLink>
    </template>

    <template #right>
      <UColorModeButton size="sm" />
    </template>
  </UFooter>
</template>
