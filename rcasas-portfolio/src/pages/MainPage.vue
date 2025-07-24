<template>
  <div class="h-auto 2xl:pt-[50px] lg:pt-[120px] 3xl:pt-[80px] xs:pt-[80px] sm:pt-[120px] overflow-hidden">
    <section class="hero-section">
    <div id="main" class=" xl:px-[125px] 2xl:h-auto xs:px-3 sm:px-3 px-5">
      <div class="flex flex-col min-h-screen items-center justify-center lg:mb-[100px]">
        <div class="col-md-8 w-full flex flex-col justify-center items-center font-gellix">
          <div class="">
            <img src="" class="logo" alt="">
            <div class="title-text font-gellix">
              <h1 class="text-white font-gellix">Reymart Casas</h1>
              <p class="sub-title">Digital Tech Developer</p>
              <p class="description">As a front-end developer from the Philippines, I'm driven by a passion for crafting web applications and finding innovative solutions to complex challenges.</p>
              <div class="">
                <a href="/" class="about-link">More about me</a>
                <img src="" alt="" class="greater-than-icon">
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
