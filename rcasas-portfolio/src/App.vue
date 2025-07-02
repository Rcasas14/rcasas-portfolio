
<template>
  <div class="min-h-screen bg-gradient-to-br from-blue-400 to-purple-600 flex items-center justify-center">
    <div class="bg-white rounded-xl shadow-2xl p-8 max-w-md">
      <h1 class="text-3xl font-bold text-gray-800 mb-4">Tailwind Test</h1>
      <p class="text-gray-600 mb-6">If this looks styled, Tailwind CSS v4 is working!</p>
      <button class="w-full bg-blue-500 hover:bg-blue-600 text-white font-semibold py-3 px-6 rounded-lg transition duration-200">
        Beautiful Button
      </button>
    </div>
  </div>
</template>

<script setup>

</script>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
