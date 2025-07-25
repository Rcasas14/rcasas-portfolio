<template>
  <!-- Footer start -->
  <footer class="footer-bg bg-gradient-to-t h-[142px] w-full relative flex">
    <div class="w-full lg:m-auto sm:mx-5 xl:h-[300px] lg:p-8">
      <!-- <div class="flex sm:flex-row xs:flex-col xs:justify-center xs:items-start sm:justify-between sm:items-center sm:mx-auto xs:m-0 h-[142px] xs:gap-y-3 xs:mx-5"> -->
        <div class="flex flex-row m-auto items-start justify-between">
        <div class="logo flex-2 font-[Gellix]">
              <a href="#"><h1 class="rcasas-logo font-gellix lg:text-2xl md:text-xl font-bold text-[#fff]">Reymart.</h1></a>
              <p class="all-rights text-[#fff]/50 text-[11px] lg:text-base md:text-sm tracking-normal pt-2">Built with dedication and a side of espresso in the Philippines, built with Vue.js</p>
              <p class="all-rights text-[#fff]/30 text-[11px] tracking-normal pt-2 ">© 2025 Reymart Casas. All rights reserved.</p>
        </div>
        <div class="important-links flex-1 font-[Gellix]">
          <p class="title text-white font-semibold">Important Links</p>
            <div class="important-links-items-div flex flex-col gap-y-2">
              <router-link class="important-links-item text-gray-400" to="/">Home</router-link>
              <router-link class="important-links-item text-gray-400" to="">Projects</router-link>
              <router-link class="important-links-item text-gray-400" to="">Technologies</router-link>
              <router-link class="important-links-item text-gray-400" to="">Contact</router-link>
              <router-link class="important-links-item text-gray-400" to="">Resume</router-link>
            </div>
        </div>
        <div class="important-links flex-1 font-[Gellix]">
          <p class="title text-white font-semibold">Social</p>
            <div class="social-div flex flex-col gap-y-2">
              <router-link class="social-item text-gray-400" to="">Github</router-link>
              <router-link class="social-item text-gray-400" to="">LinkendIn</router-link>
            </div>
        </div>

        </div>
      </div>
    </footer>
  <!-- Footer end -->
</template>

<script>
export default {
  methods: {
    isMobile() {
      return window.innerWidth < 1024;
    },
  },
};
</script>

<style scope></style>
