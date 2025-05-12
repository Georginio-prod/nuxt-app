<template>
  <div>
    <!-- Sidebar fixe -->
    <aside class="fixed top-0 left-0 z-40 w-64 h-screen transition-transform -translate-x-full sm:translate-x-0" aria-label="Sidebar">
      <div class="h-full px-3 py-4 overflow-y-auto bg-white border-r border-gray-200">
        <div class="mb-6 px-2 py-3">
          <h1 class="text-lg font-bold text-gray-900">DASHBOARD</h1>
        </div>
        
        <!-- Section Articles -->
        <div class="mb-4">
          <button @click="toggleSection('article')" class="flex items-center w-full p-2 text-gray-900 rounded-lg hover:bg-gray-100">
            <span class="inline-flex items-center">
              <BookOpenIcon class="w-5 h-5 mr-2" />
              Article
            </span>
            <ChevronDownIcon v-if="!openSections.article" class="w-4 h-4 ml-auto" />
            <ChevronUpIcon v-else class="w-4 h-4 ml-auto" />
          </button>
          <div v-if="openSections.article" class="pl-4 mt-1">
            <NuxtLink to="/articles" class="flex items-center p-2 text-gray-700 rounded-lg hover:bg-gray-100">
              List
            </NuxtLink>
            <NuxtLink to="/articles/add" class="flex items-center p-2 text-gray-700 rounded-lg hover:bg-gray-100">
              Add article
            </NuxtLink>
            <NuxtLink to="/articles/suite" class="flex items-center p-2 text-gray-700 rounded-lg hover:bg-gray-100">
              Ainsi de suite
            </NuxtLink>
          </div>
        </div>
        
        <!-- Section Catégories -->
        <div class="mb-4">
          <button @click="toggleSection('category')" class="flex items-center w-full p-2 text-gray-900 rounded-lg hover:bg-gray-100">
            <span class="inline-flex items-center">
              <TagIcon class="w-5 h-5 mr-2" />
              Category
            </span>
            <ChevronDownIcon v-if="!openSections.category" class="w-4 h-4 ml-auto" />
            <ChevronUpIcon v-else class="w-4 h-4 ml-auto" />
          </button>
          <div v-if="openSections.category" class="pl-4 mt-1">
            <NuxtLink to="/categories" class="flex items-center p-2 text-gray-700 rounded-lg hover:bg-gray-100">
              List
            </NuxtLink>
            <NuxtLink to="/categories/label1" class="flex items-center p-2 text-gray-700 rounded-lg hover:bg-gray-100">
              Label
            </NuxtLink>
            <NuxtLink to="/categories/label2" class="flex items-center p-2 text-gray-700 rounded-lg hover:bg-gray-100">
              Label
            </NuxtLink>
          </div>
        </div>
        
        <!-- Section Tags -->
        <div class="mb-4">
          <button @click="toggleSection('tags')" class="flex items-center w-full p-2 text-gray-900 rounded-lg hover:bg-gray-100">
            <span class="inline-flex items-center">
              <TagsIcon class="w-5 h-5 mr-2" />
              Tags
            </span>
            <ChevronDownIcon v-if="!openSections.tags" class="w-4 h-4 ml-auto" />
            <ChevronUpIcon v-else class="w-4 h-4 ml-auto" />
          </button>
          <div v-if="openSections.tags" class="pl-4 mt-1">
            <NuxtLink to="/tags" class="flex items-center p-2 text-gray-700 rounded-lg hover:bg-gray-100">
              List
            </NuxtLink>
            <NuxtLink to="/tags/label1" class="flex items-center p-2 text-gray-700 rounded-lg hover:bg-gray-100">
              Label
            </NuxtLink>
            <NuxtLink to="/tags/label2" class="flex items-center p-2 text-gray-700 rounded-lg hover:bg-gray-100">
              Label
            </NuxtLink>
          </div>
        </div>
      </div>
    </aside>
    
    <!-- Header fixe -->
    <header class="fixed top-0 z-30 w-full bg-white border-b border-gray-200 sm:ml-64 sm:w-[calc(100%-16rem)]">
      <div class="px-4 py-3 flex justify-end items-center">
        <div class="flex items-center space-x-4">
          <button class="p-1 rounded-full hover:bg-gray-100">
            <BellIcon class="w-6 h-6 text-gray-500" />
          </button>
          <div class="w-8 h-8 rounded-full bg-gray-200 overflow-hidden">
            <img src="https://hebbkx1anhila5yf.public.blob.vercel-storage.com/placeholder-ob7miW3mUreePYfXdVwkpFWHthzoR5.svg?height=32&width=32" alt="User profile" class="w-full h-full object-cover" />
          </div>
        </div>
      </div>
    </header>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import { 
  BookOpenIcon, 
  TagIcon, 
  BellIcon, 
  ChevronDownIcon, 
  ChevronUpIcon
} from 'lucide-vue-next'

// État pour gérer l'ouverture/fermeture des sections
const openSections = ref({
  article: true,
  category: false,
  tags: false
})

// Fonction pour basculer l'état d'une section
const toggleSection = (section) => {
  openSections.value[section] = !openSections.value[section]
}
</script>