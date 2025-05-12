<script setup lang="ts">
import type { NavigationMenuItem } from "@nuxt/ui";

const items = ref<NavigationMenuItem[]>([
  {
    icon: "i-lucide-user-round",
    to: "/",
    target: "_blank",
  },
  {
    icon: "i-lucide-bell-ring",
    to: "/",
    disabled: true,
  },
]);
</script>

<template>
  <div>
    <header class="fixed top-0 z-30 bg-backg sm:ml-64 w-full">
      <div class="px-9 py-5 flex justify-between border-b items-center">
        <div class="mb-6 px-2 py-3">
          <h1 class="text-lg font-bold text-gray-900">DASHBOARD</h1>
        </div>
        <div >
          <UNavigationMenu :items="items" class="w-full justify-center " />
        </div>
      </div>
    </header>
  </div>
</template>



<!-- <script setup lang="ts">

<template>
  <div>
    <header class="fixed top-0 z-30 bg-backg sm:ml-64 w-full">
      <div class="px-9 py-5 flex justify-between border-b items-center">
        <div class="mb-6 px-2 py-3">
          <h1 class="text-lg font-bold text-gray-900">DASHBOARD</h1>
        </div>
        <div class="flex items-center gap-5">
          <button class="p-1 rounded-full hover:bg-gray-100">
            <BellIcon class="w-6 h-6 text-gray-500" />
          </button>
          <div class="w-8 h-8 rounded-full overflow-hidden">
            <UAvatar src="https://github.com/benjamincanac.png" />
          </div>
        </div>
      </div>
    </header>
  </div>
</template>

<script setup>
import { BellIcon } from "lucide-vue-next";
// eslint-disable-next-line @typescript-eslint/no-unused-vars
import { ref } from "vue";
</script>
-->
