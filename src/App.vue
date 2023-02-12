<script setup>
import NavigationBar from './components/NavigationBar.vue'
import Main from './components/Main.vue'
</script>

<template>
  <NavigationBar/>
  <Main />
  
  <RouterView />
</template>
