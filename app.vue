<template>
  <div class="min-h-screen bg-gray-50">
    <Navbar />
    <main class="p-4 md:ml-64 pt-20 h-screen">
      <NuxtPage />
    </main>
  </div>
</template>

<script setup>
import Navbar from '~/components/Navbar.vue';
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');

html, body {
  font-family: 'Inter', sans-serif;
}
</style>