<script setup>
    import { onMounted } from 'vue' 
    import Mainsearch from '@/components/Mainsearch.vue'
    import MainCards from '@/components/MainCards.vue'
    import Mainpagination from '@/components/MainPagination.vue'

    import useAPI from '@/composables/useAPI'
    
    const { getEmployees, loading } = useAPI() 


    onMounted(async () => {
          await getEmployees()
        })
</script>

<template>
  <p v-if="loading">Loading... </p>
  <div v-else class="wrapper">
    <Mainsearch />
    <MainCards />
    <Mainpagination />
  </div>
</template>

<style scoped lang="postcss">
  .wrapper {
    @apply container mx-auto flex flex-col gap-4 py-4;
  }
</style>