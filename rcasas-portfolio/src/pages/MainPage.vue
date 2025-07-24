<template>
  <div class="h-auto 2xl:pt-[50px] lg:pt-[120px] 3xl:pt-[80px] xs:pt-[80px] sm:pt-[120px] overflow-hidden">
    <section class="hero-section">
    <div id="main" class=" xl:px-[125px] 2xl:h-auto xs:px-3 sm:px-3 px-5">
      <div class=" flex flex-col min-h-screen items-center justify-center lg:mb-[100px]">
        <div class="relative col-md-8 w-full flex flex-col justify-center items-center font-gellix">
          <img :src="backgroundGridIcon" class="background-grid w-full p-0" alt="">
          <div class="absolute flex gap-x-10 justify-around mb-21">
            <img :src="rcasasLogo" class="logo mx-10" alt="">
            <div class="title-text w-[500px]">
              <h1 class="text-white text-[36px] font-semibold py-0">Reymart Casas</h1>
              <p class="sub-title text-gray-300 text-[20px] font-semibold pt-2">Digital Tech Developer</p>
              <p class="description text-gray-300 pt-2">As a front-end developer from the Philippines, I'm driven by a passion for crafting web applications and finding innovative solutions to complex challenges.</p>
              <div class="flex flex-row items-center gap-x-2 pt-4">
                <a href="/" class="about-link text-white font-semibold">More about me</a>
                <img :src="arrowLeft" alt="" class="greater-than-icon pt-1">
              </div>
            </div>
          </div>

        </div>
      </div>
    </div>
  </section>





</div>
</template>

<script>

//import ContactForm from '@/sections/ContactForm.vue';

export default {
  components: {

  },
  data() {
    return {
      backgroundGridIcon : new URL('@/assets/background-grid.svg', import.meta.url).href,
      rcasasLogo: new URL('@/assets/rcasas-logo.svg', import.meta.url).href,
      arrowLeft: new URL('@/assets/arrow-left.svg', import.meta.url).href,

      mobileMenuOpen: false,
    }
}
};
</script>

<style scoped>
</style>
