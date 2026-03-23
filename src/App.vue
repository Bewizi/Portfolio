<script setup lang="ts">
import { RouterView } from 'vue-router'
import App_header from './components/app_header.vue'
import App_footer from './components/app_footer.vue'
// import App_container from './components/app_container.vue'
</script>

<template>
  <!-- <App_container></App_container> -->
  <App_header />
  <RouterView />
  <App_footer />
</template>
