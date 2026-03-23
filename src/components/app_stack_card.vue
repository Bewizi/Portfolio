<script setup lang="ts">
import { computed } from 'vue'

const props = defineProps<{
  title: string
  icon: string
  description: string
  borderColor: 'blue-400' | 'orange-500' | 'green-500'
}>()

const borderClass = computed(() => {
  return (
    {
      'blue-400': 'border-blue-400',
      'orange-500': 'border-orange-500',
      'green-500': 'border-green-500',
    }[props.borderColor] || ''
  )
})

const iconSrc = computed(() => new URL(`../assets/icons/${props.icon}.svg`, import.meta.url).href)
</script>

<template>
  <div class="border-l-4 bg-card-background p-3 rounded-md" :class="borderClass">
    <img :src="iconSrc" alt="icon" class="w-10 h-10 mb-3" />
    <h3 class="text-xl font-bold mb-2 text-text-primary">{{ title }}</h3>
    <p class="text-text-secondary">{{ description }}</p>
  </div>
</template>
