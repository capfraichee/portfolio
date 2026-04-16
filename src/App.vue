<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div class="grid grid-cols-12 content-start gap-1 px-25 min-h-screen">
    <header class="ml-2 col-span-12 h-15 align-center flex items-center mt-20">
      <nav class="flex flex-row gap-6" style="font-family: 'Mulish', sans-serif; font-weight: 600; text-transform: uppercase; font-size: 20px;">
        <RouterLink to="/" class="p-2 rounded">Hjernen bag</RouterLink>
        <!-- <RouterLink to="/about" class="p-2 rounded">Mig</RouterLink> -->
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
nav {
  align-items: center;
}

nav a {
  display: inline-block;
  position: relative;
  color: rgba(255, 255, 255, 0.45);
  text-decoration: none;
  transform-origin: center bottom;
  transition: color 0.2s ease, transform 0.2s ease;
}

nav a:hover {
  color: var(--text-color);
  background-color: transparent;
}

nav a.router-link-exact-active {
  color: var(--text-color);
  transform: scale(1.1);
}

nav a.router-link-exact-active::after {
  content: '';
  position: absolute;
  left: 50%;
  bottom: -8px;
  width: 7px;
  height: 7px;
  border-radius: 9999px;
  transform: translateX(-50%);
  background-color: var(--text-color);
}
</style>
