<template>
  <div
    class="text-center md:grid md:grid-cols-2 lg:grid-cols-3 md:gap-12 space-y-4 md:space-y-0"
  >
    <div>
      <div
        class="flex justify-center items-center mx-auto mb-4 w-10 h-10 bg-gray-100 rounded-lg dark:bg-gray-800 lg:h-16 lg:w-16"
      >
        <UIcon
          name="i-heroicons-envelope"
          class="w-5 h-5 text-primary-600 lg:w-8 lg:h-8"
          dynamic
        />
      </div>
      <p class="mb-2 text-xl font-bold dark:text-white">Napisz do nas:</p>
      <p class="mb-3 text-gray-500 dark:text-gray-400">
        Napisz do nas, aby uzyskać odpowiedzi na swoje pytania i zapytania.
      </p>
      <NuxtLink
        to="mailto:malopolska134@wp.pl"
        class="font-semibold text-primary-600 dark:text-primary-500 hover:underline"
        >malopolska134@wp.pl</NuxtLink
      >
    </div>
    <div>
      <div
        class="flex justify-center items-center mx-auto mb-4 w-10 h-10 bg-gray-100 rounded-lg dark:bg-gray-800 lg:h-16 lg:w-16"
      >
        <UIcon
          name="i-heroicons-phone"
          class="w-5 h-5 text-primary-600 lg:w-8 lg:h-8"
          dynamic
        />
      </div>
      <p class="mb-2 text-xl font-bold dark:text-white">Zadzwoń pod:</p>
      <p class="mb-3 text-gray-500 dark:text-gray-400">
        Chętnie odpowiemy na Twoje pytania i zapytania telefonicznie.
      </p>
      <NuxtLink
        to="tel:+48324732353"
        class="font-semibold text-primary-600 dark:text-primary-500"
        >+48 32 473 23 53</NuxtLink
      >
    </div>
    <div>
      <div
        class="flex justify-center items-center mx-auto mb-4 w-10 h-10 bg-gray-100 rounded-lg dark:bg-gray-800 lg:h-16 lg:w-16"
      >
        <UIcon
          name="i-heroicons-map-pin"
          class="w-5 h-5 text-primary-600 lg:w-8 lg:h-8"
          dynamic
        />
      </div>
      <p class="mb-3 text-xl font-bold dark:text-white">Lokalizacja</p>
      <p class="mb-3 text-gray-500 dark:text-gray-400">
        Sprawdź naszą lokalizację i odwiedź nas w dogodnym dla Ciebie terminie.
      </p>
      <NuxtLink
        to="https://maps.app.goo.gl/oARugnYMTsL1HTmA8"
        target="_blank"
        class="inline-flex py-2 px-4 text-sm font-medium text-center rounded-lg border text-primary-600 border-primary-600 hover:text-white hover:bg-primary-600 focus:ring-4 focus:outline-none focus:ring-primary-300 dark:border-primary-500 dark:text-primary-500 dark:hover:text-white dark:hover:bg-primary-600 dark:focus:ring-primary-800"
        >Małopolska 134 44-335 Jastrzębie-Zdrój</NuxtLink
      >
    </div>
  </div>
</template>
