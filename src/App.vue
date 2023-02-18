<script setup>
import NavigationBar from '@/components/NavigationBar.vue'
import MainPage from '@/components/MainPage.vue'
</script>

<template>
  <NavigationBar/>
  <MainPage />
  
  <RouterView />
</template>
