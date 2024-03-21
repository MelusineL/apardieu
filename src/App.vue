<template>
  <header class="relative w-full">
    <NavBar />
  </header>

  <RouterView />
</template>

<script setup>
import { RouterView } from 'vue-router'
import NavBar from '../src/components/NavBar.vue'
</script>
