<template>
  <div class="container mx-auto h-screen flex flex-col">
    <header class="px-3 py-6 bg-gray-200 flex">
      <div class="text-2xl font-semibold leading-none absolute ">
        Beer
      </div>
      <MainNavigation/>
    </header>
    <main class="h-full bg-gray-100 p-3">
      <Nuxt />
    </main>
    <footer class="px-3 py-6 bg-gray-500 text-white text-center">
      copyright 2024
    </footer>
  </div>
</template>

<script setup lang="ts">
import MainNavigation from "~/components/MainNavigation.vue";

</script>