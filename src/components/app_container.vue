<template>
  <section :class="`max-w-7xl mx-auto px-5 py-8 ${$props.class || ''}`">
    <slot />
  </section>
</template>

<script setup lang="ts">
defineProps<{
  class?: string
}>()
</script>

<style scoped></style>
