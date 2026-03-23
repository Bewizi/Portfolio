<template>
  <App_container class="flex items-center justify-between">
    <header class="py-6">
      <h1 class="text-3xl font-bold text-primary-accent">TOLUWALASE BEWAJI</h1>
    </header>
    <nav class="flex items-center gap-5">
      <ul class="flex gap-4 text-text-primary">
        <li><App_link to="/">Home</App_link></li>
        <li><App_link to="/about">About</App_link></li>
        <li><App_link to="/contact">Contact</App_link></li>
      </ul>
      <App_link to="/resume">
        <App_botton :is-bg-color="true">Resume</App_botton>
      </App_link>
    </nav>
  </App_container>
</template>

<script setup lang="ts">
import App_botton from './app_botton.vue'
import App_container from './app_container.vue'
import App_link from './app_link.vue'
</script>

<style scoped></style>
