<template>
  <div class="px-16">
    <SectionTitle title="Portfolio" />
    <MasonryGrid :items="projects" />
  </div>
</template>

<script setup>
import SectionTitle from '../elements/SectionTitle.vue'
import MasonryGrid from '../modules/MasonryGrid.vue'

const projects = [
  {
    id: 0,
    name: 'Beyond The Last Frontier'
  },
  {
    id: 1,
    name: 'Cooldown'
  },
  {
    id: 2,
    name: 'Crossroads'
  },
  {
    id: 3,
    name: 'Delta Race'
  },
  {
    id: 4,
    name: 'Ion Odyssey'
  },
  {
    id: 5,
    name: 'SpilledBeer'
  }
]
</script>
