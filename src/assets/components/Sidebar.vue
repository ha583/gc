<template>
  <div :class="['fixed inset-y-0 left-0 bg-gray-800 p-4 space-y-4 z-10 sidebar', { open: sidebarOpen }]">
    <div class="flex items-center justify-between">
      <div class="flex items-center">
        <h1 class="text-xl font-bold text-gray-200">Tuesday AI</h1>
        <button @click="toggleHistorySidebar" class="ml-3 text-gray-400 hover:text-gray-200">
          <i class="fas fa-history"></i>
        </button>
      </div>
      <button @click="toggleSidebar" class="text-gray-400 hover:text-gray-200">
        <i class="fas fa-times"></i>
      </button>
    </div>
    <nav class="flex flex-col space-y-2">
      <a href="#" class="flex items-center px-2 py-1 hover:bg-gray-700 rounded transition duration-200">
        <i class="fas fa-home mr-3"></i>
        Home
      </a>
      <a href="#" class="flex items-center px-2 py-1 hover:bg-gray-700 rounded transition duration-200">
        <i class="fas fa-user mr-3"></i>
        Profile
      </a>
      <a href="#" class="flex items-center px-2 py-1 hover:bg-gray-700 rounded transition duration-200">
        <i class="fas fa-cog mr-3"></i>
        Settings
      </a>
      <a href="#" class="flex items-center px-2 py-1 hover:bg-gray-700 rounded transition duration-200">
        <i class="fas fa-sign-in-alt mr-3"></i>
        Login/Signup
      </a>
    </nav>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'

const sidebarOpen = ref(false)

const toggleSidebar = () => {
  sidebarOpen.value = !sidebarOpen.value
}

const toggleHistorySidebar = () => {
  // Implement the logic to toggle history sidebar
}
</script>

<style scoped>
.sidebar {
  transform: translateX(-250px);
  transition: transform 0.3s ease-in-out;
}

.sidebar.open {
  transform: translateX(0);
}
</style>
