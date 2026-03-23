<script setup lang="ts">
import App_botton from '@/components/app_botton.vue'
import App_card from '@/components/app_card.vue'
import App_container from '@/components/app_container.vue'
import App_link from '@/components/app_link.vue'
import App_stack_card from '@/components/app_stack_card.vue'
</script>

<template>
  <main>
    <!-- hero section -->
    <App_container>
      <h1 class="text-6xl font-bold mb-6 uppercase">
        <span class="text-text-primary"> Building fast, </span>

        <span class="text-primary-accent"> scalable mobile apps with Flutter. </span>
      </h1>
      <p class="text-text-secondary text-2xl mb-6">
        I’m Toluwalase — a Flutter developer specializing in Firebase and Supabase. I create
        responsive, high-performance mobile applications with clean UI and reliable backend systems.
      </p>
      <!-- two buttons will wrap inside div and use flex create a custom button -->
      <div class="flex gap-4">
        <App_botton :is-bg-color="true"> View My Work </App_botton>
        <App_link to="/contact">
          <App_botton :is-border="true"> Contact Me </App_botton>
        </App_link>
      </div>
    </App_container>

    <!-- tech stack section -->
    <App_container class="mt-20">
      <h2 class="text-4xl font-bold text-text-primary mb-6">The Technical Stack</h2>
      <p class="text-text-secondary text-lg mb-4">
        I work primarily with <strong class="text-primary-accent"> Flutter </strong> for frontend
        development, leveraging its powerful UI toolkit to create beautiful and responsive mobile
        applications. For backend services, I utilize
        <strong class="text-primary-accent"> Firebase </strong>
        and

        <strong class="text-primary-accent"> Supabase </strong>
        to handle authentication, real-time data, and cloud storage efficiently.
      </p>
      <p class="text-text-secondary text-lg">
        My expertise in these technologies allows me to build scalable, high-performance apps that
        deliver real value to users.
      </p>

      <!-- tech stack cards will wrap inside div and use grid to create a custom card -->
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 mt-8">
        <App_stack_card
          title="Flutter"
          icon="icon_flutter"
          description="Flutter is a powerful UI toolkit that allows me to create beautiful and responsive mobile applications with a single codebase."
          border-color="blue-400"
        />
        <App_stack_card
          title="Firebase"
          icon="icon_firebase"
          description="Firebase provides a comprehensive suite of backend services, including authentication, real-time database, and cloud storage, which I use to build robust and scalable applications."
          border-color="orange-500"
        />
        <App_stack_card
          title="Supabase"
          icon="icon_supabase"
          description="Supabase is an open-source alternative to Firebase that offers powerful backend features like authentication, real-time data, and cloud storage, which I leverage to create efficient and scalable applications."
          border-color="green-500"
        />
      </div>
    </App_container>

    <!-- my work section-->
    <App_container class="mt-20" id="work">
      <h2 class="text-4xl font-bold text-text-primary mb-6">My Work</h2>
      <p class="text-text-secondary text-lg mb-4">
        I’ve had the opportunity to work on a variety of projects, from e-commerce platforms to
        location-based services. My focus is always on building apps that not only look good but
        also perform smoothly and deliver real value to users.
      </p>
      <p class="text-text-secondary text-lg">
        I’m constantly improving my skills, exploring new technologies, and pushing myself to build
        better, more impactful applications.
      </p>

      <!-- project cards will wrap inside div and use grid to create a custom card -->
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 mt-8">
        <App_card
          frontend="Flutter"
          backend="Supabase"
          projectName="HomeFinder"
          overview="HomeFinder helps users find homes across Nigeria quickly and efficiently."
          image="image"
        />
        <App_card
          frontend="Flutter"
          backend="Firebase"
          projectName="CLOT"
          overview="Clot is a mobile e-commerce application designed to simplify online clothing shopping with a clean interface and fast performance"
          image="image"
        />
      </div>
    </App_container>
  </main>
</template>
