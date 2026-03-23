<script setup lang="ts">
defineProps<{
  frontend: string
  backend: string
  projectName: string
  overview: string
  image: string
}>()
</script>

<template>
  <div class="group">
    <div
      class="bg-card-background rounded-3xl overflow-hidden hover-lift border border-primary-accent/10 transition-shadow"
    >
      <div class="h-80 bg-card-background relative">
        <img
          class="w-full h-full object-cover mix-blend-overlay opacity-60"
          data-alt="Modern mobile shopping app interface showcase"
          src="https://lh3.googleusercontent.com/aida-public/AB6AXuDo948JEcnbs93Uj43jYWS5VXKfbtDN_bFAzdmuRGCN6C0YSgXv7gTndCwopINzcgtDeEEpSvrWfHu65ZaQ58K5aWOI8nY7dK8UkO9-mUnSbaUstGVUtpGul5dJ4MArjjwAGcVohyOL3wbX8dGvv28IIasHlIEYm0qNUeqKkoccaNxcj69CM3HyzZ8yPTfRc0fheE4jUTaa1T-hF5k38Aaeuka8TodWqocPxYzbBvbaE-ja35au9c4tbQb6rprd1TedMSPYv_8fbmE4"
        />
        <div class="absolute top-6 left-6 flex gap-2">
          <span
            class="bg-primary-accent text-text-primary text-xs font-bold px-3 py-1 rounded-full border border-primary-accent/20"
            >{{ frontend }}</span
          >
          <span
            class="bg-primary-accent text-text-primary text-xs font-bold px-3 py-1 rounded-full border border-primary-accent/20"
            >{{ backend }}</span
          >
        </div>
      </div>
      <div class="p-10">
        <h3 class="font-headline text-3xl text-text-primary font-extrabold mb-4">
          {{ projectName }}
        </h3>
        <p class="text-on-surface-variant leading-relaxed mb-8 text-text-secondary">
          {{ overview }}
        </p>
        <button class="flex items-center gap-3 text-primary-accent font-bold group">
          View Project
          <span
            class="material-symbols-outlined text-sm bg-primary/10 p-2 rounded-full group-hover:bg-primary group-hover:text-on-primary transition-colors"
            >open_in_new</span
          >
        </button>
      </div>
    </div>
  </div>
</template>
