<template>
  <div
    class="flex-row items-center justify-between px-6 pt-14 md:px-12 lg:px-24 py-24 sm:py-32 lg:py-48"
  >
    <div class="flex-col gap-4 max-w-xl">
      <div class="text-left">
        <h1 class="text-4xl font-bold tracking-tight text-gray-900 sm:text-6xl">
          {{ name }}
        </h1>
        <h2 class="mt-4 text-2xl font-bold tracking-tight text-gray-900 sm:text-4xl">
          {{ title }}
        </h2>
        <p class="mt-4 text-base leading-8 text-gray-600">
          {{ presentation }}
        </p>
      </div>
      <div class="mt-10 flex items-center gap-x-6">
        <button
          class="rounded-md bg-indigo-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
        >
          Mon portfolio
        </button>
      </div>
    </div>
  </div>
</template>

<script setup>
const name = 'Arthur Pardieu'
const title = 'Ingénieur informatique / Développeur web'
const presentation =
  'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam mollis ultrices neque, in tempor turpis tristique sit amet. Quisque mauris est, semper sed ligula ac, aliquet eleifend odio. Suspendisse egestas ex quis ex sollicitudin tincidunt sed et velit. Nulla sit amet velit finibus, mollis metus nec, ullamcorper odio. Duis vel cursus sapien, vitae dapibus mauris. Nulla sed magna lorem. Phasellus tempus semper mauris a posuere. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum in urna massa.'
</script>
