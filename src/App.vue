<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div 
    :class="[
      'grid grid-cols-12 content-start gap-1 px-25 min-h-screen relative',
      $route.path === '/' ? 'bg-black' : 'bg-[var(--background-color-dark)]'
    ]"
  >
    <header v-if="$route.path !== '/'" class="absolute top-0 left-0 w-full h-[70px] z-50 flex items-center px-39 border-b-[2px] border-black">
      <nav class="flex flex-row gap-6" style="font-family: 'Mulish', sans-serif; font-weight: 400; font-size: 14px;">
        <RouterLink to="/" class="p-2 rounded">Forside</RouterLink>
        <RouterLink to="/about" class="p-2 rounded">Om mig</RouterLink>
        <RouterLink to="/school-projects" class="p-2 rounded ">Skole Projekter</RouterLink>
        <RouterLink to="/personal-projects" class="p-2 rounded ">Personlige Projekter</RouterLink>
      </nav>
    </header>

    <main :class="['col-span-12', $route.path !== '/' ? 'pt-[70px]' : '']">
      <RouterView />
    </main>
  </div>
</template>

<style scoped>
nav a.router-link-exact-active {
  color: var(--text-color);
  text-decoration: underline;
}
</style>
