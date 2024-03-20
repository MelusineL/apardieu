<template>
  <div
    class="flex flex-row items-center justify-between px-6 md:px-12 lg:px-32 py-16 sm:py-18 lg:py-28"
  >
    <div class="flex flex-col gap-6 lg:gap-8 max-w-xl">
      <div class="text-left">
        <h1 class="text-4xl font-semibold tracking-tight uppercase text-orange-700 sm:text-6xl">
          {{ name }}
        </h1>
        <h2 class="mt-4 text-2xl font-medium tracking-tight text-orange-800 sm:text-4xl">
          {{ title }}
        </h2>
        <p class="mt-2 text-base text-slate-800">
          {{ presentation }}
        </p>
      </div>
      <div class="flex items-center gap-x-6">
        <a
          href="#"
          class="rounded-md bg-sky-500 px-3.5 py-2.5 text-sm font-medium text-white shadow-sm hover:bg-sky-400 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-sky-500"
        >
          Mon portfolio
        </a>
      </div>
    </div>
    <div>
      <img
        class="rounded-md h-[550px]"
        src="https://anniversaire-celebrite.com/upload/250x333/monsieur-propre-250.jpg"
        alt="Portrait d'Arthur PARDIEU"
      />
    </div>
  </div>
</template>

<script setup>
const name = 'Arthur Pardieu'
const title = 'Ingénieur informatique / Développeur web'
const presentation =
  'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam mollis ultrices neque, in tempor turpis tristique sit amet. Quisque mauris est, semper sed ligula ac, aliquet eleifend odio. Suspendisse egestas ex quis ex sollicitudin tincidunt sed et velit. Nulla sit amet velit finibus, mollis metus nec, ullamcorper odio. Duis vel cursus sapien, vitae dapibus mauris. Nulla sed magna lorem. Phasellus tempus semper mauris a posuere. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Vestibulum in urna massa.'
</script>
