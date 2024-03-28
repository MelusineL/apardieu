<template>
  <div class="grid gap-6">
    <ProjectCard v-for="item in props.items" :key="item.id" />
  </div>
</template>

<script setup>
import ProjectCard from '../elements/ProjectCard.vue'

const props = defineProps({
  items: {
    type: Array,
    default: () => []
  }
})
</script>
