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
    <header v-if="$route.path !== '/'" class="fixed top-0 left-0 w-[100vw] h-[70px] z-[999] bg-[var(--background-color-dark)] flex items-center justify-center md:justify-start border-b-[2px] border-black md:pl-[100px]">
      <nav class="flex flex-row gap-6 custom-nav-align" style="font-family: 'Mulish', sans-serif; font-weight: 400; font-size: 14px;">
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

/* Sikrer centreret på små skærme */
.custom-nav-align {
  width: 100%;
  justify-content: center;
}

/* Skubber det venstre på desktop */
@media (min-width: 768px) {
  .custom-nav-align {
    justify-content: flex-start !important;
  }
}
</style>
