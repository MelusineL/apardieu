<template>
  <div class="w-full py-2 border-b-2 border-slate-200">
    <h2 class="text-3xl text-slate-900 font-medium">
      {{ props.title }}
    </h2>
  </div>
</template>

<script setup>
const props = defineProps({
  title: {
    type: String,
    required: true
  }
})
</script>
