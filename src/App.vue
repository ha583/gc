<template>
  <div class="flex">
    <Sidebar />
    <ChatContainer />
  </div>
</template>

<script lang="ts" setup>
import Sidebar from './assets/components/Sidebar.vue'
import ChatContainer from './assets/components/ChatContainer.vue'
</script>

<style>
body {
  font-family: 'Inter', sans-serif;
  margin: 0;
  padding: 0;
  background-color: #1A202C;
  color: #E2E8F0;
}
</style>

