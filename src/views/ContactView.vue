<script setup lang="ts">
import App_container from '@/components/app_container.vue'
</script>

<template>
  <App_container class="py-32 px-8 max-w-7xl mx-auto mb-20" id="contact">
    <div class="bg-card-background rounded-4xl p-12 md:p-24 text-center">
      <span
        class="font-headline text-primary-accent font-bold tracking-[0.2em] uppercase text-sm mb-6 block"
        >Ready to start?</span
      >
      <h2
        class="font-headline text-4xl md:text-6xl font-extrabold tracking-tighter mb-10 max-w-3xl mx-auto text-text-primary"
      >
        Let’s build your next <span class="text-primary-accent">big idea</span> together.
      </h2>
      <div class="flex flex-col md:flex-row gap-6 justify-center items-center">
        <a
          class="bg-primary-accent text-text-primary px-10 py-5 rounded-md font-bold text-lg hover:scale-105 transition-transform flex items-center gap-3"
          href="mailto:hello@kinetic.dev"
        >
          <span class="material-symbols-outlined">mail</span> Get in Touch
        </a>
        <div class="flex gap-4">
          <a
            class="p-4 bg-primary-accent rounded-md text-[#c2c6d2] hover:text-[#81cfff] transition-colors"
            href="#"
          >
            <span class="material-symbols-outlined">link</span>
          </a>
          <a
            class="p-4 bg-primary-accent rounded-md text-[#c2c6d2] hover:text-[#81cfff] transition-colors"
            href="#"
          >
            <span class="material-symbols-outlined">share</span>
          </a>
        </div>
      </div>
    </div>
  </App_container>
</template>
