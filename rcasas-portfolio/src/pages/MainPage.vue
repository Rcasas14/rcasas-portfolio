<template>
  <div class="h-auto 2xl:pt-[50px] lg:pt-[120px] 3xl:pt-[80px] xs:pt-[80px] sm:pt-[120px] overflow-hidden h-full">
    <section class="hero-section">
      <div id="main" class=" xl:px-[125px] 2xl:h-auto xs:px-3 sm:px-3 px-5">
      <div class="relative flex flex-col min-h-screen items-center justify-center lg:mb-[100px]">
        <div class="absolute col-md-8 w-full flex flex-col justify-center items-center font-gellix">
          <img :src="backgroundGridIcon" class="background-grid w-full p-0" alt="">
          <div class="absolute flex gap-x-21 justify-around items-center mb-21">
            <img :src="rcasasLogo" class="logo mx-10 2xl:h-full 2xl:w-[310px]" alt="">
            <div class="title-text w-[500px] font-[Gellix]">
              <h1 class="text-white xs:text-[24px] md:text-[36px] xl:text-[42px] 2xl:text-[64px] font-extrabold py-0 ">Reymart Casas</h1>
              <p class="sub-title text-gray-300 text-[20px] font-semibold pt-2">Digital Tech Developer</p>
              <p class="description text-gray-300 pt-2">As a front-end developer from the Philippines, I'm driven by a passion for crafting web applications and finding innovative solutions to complex challenges.</p>
                <a href="/" class="flex flex-row items-center gap-x-2 pt-4">
                  <p class="about-link text-white font-semibold xs:text-[18px] md:text-[20px] pb-1">More about me</p>
                  <img :src="arrowLeft" alt="" class="greater-than-icon pt-1">
                </a>
            </div>
          </div>

        </div>
      </div>
    </div>
  </section>

  <about-page></about-page>





</div>
</template>

<script>
import AboutPage from './AboutPage.vue';
//import ContactForm from '@/sections/ContactForm.vue';

export default {
  components: {
    AboutPage,

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
