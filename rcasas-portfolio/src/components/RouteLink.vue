<template>
    <router-link
    :to="to"
    class="relative flex items-center px-5 py-0 text-xs duration-150 ease-in-out group  "
    :class="{
      'bg-light-gradient bg-no-repeat bg-[length:200%_100%] ': isActive
    }"
    @mouseenter="isHovered = true"
    @mouseleave="isHovered = false"
  >
    <p class="tracking-normal font-medium text-[16px] text-white border-b-1 border-transparent hover:border-gray-300 transition-all duration-300 ease-in-out">{{ label }}</p>
  </router-link>
  </template>

  <script>
  export default {
    props: {
      to: { type: String, required: true },
      label: { type: String, required: true },
      isActive: { type: Boolean, default: false },
    },
    data() {
      return {
        isHovered: false,
      };
    },
  };
  </script>

  <style scoped>
  /* Add your custom animation style here if needed */
  </style>
