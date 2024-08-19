<template>
    <div class="card">
      <p class="text-lg font-semibold">{{ text }}</p>
      <p class="text-gray-400 text-sm">{{ description }}</p>
    </div>
  </template>
  
  <script lang="ts" setup>
  defineProps<{
    text: string,
    description: string
  }>()
  </script>
  
  <style scoped>
  .card {
    background-color: #2D3748;
    padding: 1rem;
    border-radius: 0.5rem;
    box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.3);
    transition: transform 0.3s ease-in-out;
  }
  
  .card:hover {
    transform: translateY(-0.5rem);
  }
  </style>
  