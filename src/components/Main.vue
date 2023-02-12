<script setup>
    import MainSearch from './Mainsearch.vue'
    import MainCards from './MainCards.vue'
    import Mainpagination from './MainPagination.vue'
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