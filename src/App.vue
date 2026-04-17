<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div 
    :class="[
      'grid grid-cols-12 content-start gap-1 px-25 min-h-screen',
      $route.path === '/' ? 'bg-black' : 'bg-[var(--background-color-dark)]'
    ]"
  >
    <header v-if="$route.path !== '/'" class="ml-2 col-span-12 h-15 align-center flex items-center">
      <nav class="flex flex-row gap-6" style="font-family: 'Mulish', sans-serif; font-weight: 600; text-transform: uppercase; font-size: 20px;">
        <RouterLink to="/" class="p-2 rounded">Forside</RouterLink>
        <RouterLink to="/about" class="p-2 rounded">Om mig</RouterLink>
        <RouterLink to="/school-projects" class="p-2 rounded ">Skole Projekter</RouterLink>
        <RouterLink to="/personal-projects" class="p-2 rounded ">Personlige Projekter</RouterLink>
      </nav>
    </header>

    <main class="col-span-12">
      <RouterView />
    </main>
  </div>
</template>

<style scoped>

</style>
