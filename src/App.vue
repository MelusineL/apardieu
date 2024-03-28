<template>
  <header class="relative w-full">
    <NavBar />
  </header>

  <RouterView />
</template>

<script setup>
import { RouterView } from 'vue-router'
import NavBar from '../src/components/modules/NavBar.vue'
</script>
