<script setup>
import { RouterView } from 'vue-router'
import SidebarMenu from './components/layout/SidebarMenu.vue'
</script>

<template>
   <div class="flex flex-row">
    <SidebarMenu/>
    <RouterView />
  </div>
</template>

<style scoped></style>
