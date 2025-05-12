<template>
  <div class="min-h-screen bg-gray-50">
    <!-- Navbar -->
    <Navbar />

    <div class="flex">
      <Sidebar class="pt-30 pl-10" />

      <main class="flex-1 p-4 pt-20 h-screen">
        <NuxtPage />
      </main>
    </div>
  </div>
</template>

<script setup>
import Navbar from "~/components/Navbar.vue";
import Sidebar from "~/components/Sidebar.vue";
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap");

html,
body {
  font-family: "Inter", sans-serif;
}
</style>
