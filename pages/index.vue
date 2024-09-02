<template>
  <div class="relative min-h-screen bg-gray-300">
    <!-- Spiderman Component with fixed positioning -->
    <div class="fixed top-0  w-full h-screen z-10">
      <Spiderman />
    </div>

    <!-- Main Content with Scroll Effect -->
    <div class="relative "> <!-- Padding top to make space for the Spiderman component -->
      <!-- Content on the first page -->
      <section class="h-screen flex items-center justify-center text-white z-20 relative">
        <h1 class="text-4xl">This is the First Page</h1>
      </section>

      <!-- Content on the second page -->
      <section class="h-screen flex items-center justify-center text-white  z-20 relative">
        <h1 class="text-4xl">This is the Second Page</h1>
      </section>
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
/* Ensure content is not covered by Spiderman component */
section {
  position: relative;
  z-index: 20; /* Ensure content is above the Spiderman component */
}

/* Additional styling if needed */
</style>
