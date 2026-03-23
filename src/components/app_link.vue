<script setup lang="ts">
defineProps<{
  to: string
}>()
</script>

<template>
  <router-link :to="to" class="cursor-pointer hover:text-primary-accent transition-colors">
    <slot />
  </router-link>
</template>
