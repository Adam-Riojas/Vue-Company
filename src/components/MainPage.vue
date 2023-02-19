<script setup>
    import Mainsearch from '@/components/Mainsearch.vue'
    import MainCards from '@/components/MainCards.vue'
    import Mainpagination from '@/components/MainPagination.vue'
</script>

<template>
  <div class="wrapper">
    <MainSearch />
    <MainCards />
    <Mainpagination />
  </div>
</template>

<style scoped lang="postcss">
  .wrapper {
    @apply container mx-auto flex flex-col gap-4 py-4;
  }
</style>