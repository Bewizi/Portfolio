<script setup lang="ts">
import App_botton from '@/components/app_botton.vue'
import App_card from '@/components/app_card.vue'
import App_container from '@/components/app_container.vue'
import App_link from '@/components/app_link.vue'
import App_stack_card from '@/components/app_stack_card.vue'
import homeFinderImage from '@/assets/home_page.png'
import clotImage from '@/assets/clot.png'
</script>

<template>
  <main>
    <!-- hero section -->
    <App_container>
      <h1 class="text-3xl/12 lg:text-6xl/normal font-bold mb-6 uppercase">
        <span class="text-text-primary"> I build mobile apps that help </span>

        <span class="text-primary-accent"> startups launch fast and scale confidently. </span>
      </h1>
      <p class="text-text-secondary lg:text-2xl mb-6">
        I’m Toluwalase — a Flutter developer specializing in Firebase and Supabase. I build mobile
        apps that are reliable, easy to use, and ready for real users from day one.
      </p>
      <!-- two buttons will wrap inside div and use flex create a custom button -->
      <div class="flex gap-4">
        <App_botton :is-bg-color="true">
          <a href="#work"> View My Projects </a>
        </App_botton>
        <App_link to="/contact">
          <App_botton :is-border="true"> Start a Project </App_botton>
        </App_link>
      </div>
    </App_container>

    <!-- tech stack section -->
    <App_container class="mt-20">
      <h2 class="text-4xl font-bold text-text-primary mb-6">The Technical Stack</h2>
      <p class="text-text-secondary text-lg">
        I use <strong class="text-primary-accent"> Flutter </strong>,
        <strong class="text-primary-accent"> Firebase </strong> and
        <strong class="text-primary-accent"> Supabase </strong> to build apps that:
      </p>
      <ul class="list-disc list-inside mt-4 text-text-secondary">
        <li>Handle real-time data smoothly</li>
        <li>Scale as your users grow</li>
        <li>Stay reliable under load</li>
      </ul>

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
      <p class="text-text-secondary lg:text-lg mb-4">
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
          overview="Built a location-based app that helps users find available homes across Nigeria with real-time data and smart filtering."
          :image="homeFinderImage"
          alt="HomeFinder app interface showcasing real-time home listings and smart filtering features"
          link="https://github.com/Bewizi/homefinder"
          projectLink="https://drive.google.com/drive/folders/1fWTLG_zq2kA_74Ucfa55PFU-8dKRHo2m?usp=drive_link"
        />
        <App_card
          frontend="Flutter"
          backend="Firebase"
          projectName="CLOT"
          overview="Clot is a mobile e-commerce application designed to simplify online clothing shopping with a clean interface and fast performance"
          :image="clotImage"
          alt="CLOT e-commerce app interface showcasing a clean design and fast performance for online clothing shopping"
          link="https://github.com/Bewizi/clot"
          projectLink="https://drive.google.com/file/d/1JB3IpWT9JDanxHnGXfcytpRffYvdWL5i/view?usp=drive_link"
        />
      </div>
    </App_container>
  </main>
</template>
