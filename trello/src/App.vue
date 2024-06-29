<script setup>
import { RouterView } from 'vue-router'
// import Home from './views/HomeView.vue'
import SidebarMenu from './components/organisms/SidebarMenu.vue'
</script>

<template>
   <div class="flex flex-row">
    <SidebarMenu/>
    <RouterView />
  </div>
</template>

<style scoped></style>
