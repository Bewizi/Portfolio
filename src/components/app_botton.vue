<script setup lang="ts">
defineProps<{
  isBgColor?: boolean
  isBorder?: boolean
}>()
</script>

<template>
  <button
    :class="[
      'px-4 py-2 rounded transition text-white',
      isBgColor ? 'bg-primary-accent hover:bg-primary-accent/90' : 'bg-transparent',
      isBorder ? 'border border-primary-accent' : '',
    ]"
  >
    <slot />
  </button>
</template>
