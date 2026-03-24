<script setup lang="ts">
import App_container from '@/components/app_container.vue'
</script>

<template>
  <App_container class="about flex flex-col justify-center items-center min-h-screen text-center">
    <img
      src="@/assets/profile_picture.jpg"
      alt="Profile"
      class="w-36 h-36 rounded-full object-cover mx-auto mb-6 border-4 border-primary-accent"
    />
    <h1 class="text-text-primary mb-8 text-2xl font-bold">ABOUT ME</h1>
    <p class="text-text-secondary mb-6">
      I’m a Flutter developer focused on building modern mobile applications that are fast,
      scalable, and user-friendly. I work primarily with Firebase and Supabase to create powerful
      backend systems that handle authentication, real-time data, and cloud storage efficiently.
    </p>

    <p class="text-text-secondary mb-6">
      I help turn ideas into real, usable products — from concept to a working mobile app whether
      it’s an e-commerce platform or a location-based service. My goal is always to build apps that
      not only look good but also perform smoothly and deliver real value to users.
    </p>

    <p class="text-text-secondary">
      I’m constantly improving my skills, exploring new technologies, and pushing myself to build
      better, more impactful applications.
    </p>
  </App_container>
</template>
