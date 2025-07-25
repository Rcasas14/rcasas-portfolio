<!-- <template>
    <div class="h-auto 2xl:pt-[50px] lg:pt-[120px] 3xl:pt-[80px] xs:pt-[80px] sm:pt-[120px] overflow-hidden">
      <section class="about-section">
      <div id="main" class="relative xl:px-[125px] 2xl:h-auto xs:px-3 sm:px-3">

        <div class=" about-div">

        </div>
      </div>
    </section>


  </div>
  </template> -->

  <template>
  <div class="min-h-screen bg-[#1F2937] flex items-center justify-center p-4 md:p-8 relative overflow-hidden">
    <!-- Background Overlay for Depth -->
    <div class="absolute inset-0 bg-gradient-to-t from-slate-900/30 to-transparent"></div>

    <!-- Background Art - Behind Text (Middle) -->
    <div class="absolute inset-0 flex items-center justify-center z-0 opacity-20">
      <img
        :src="bgArtSeven"
        alt="Background Art"
        class="w-12 h-10 2xl:w-[123px] 2xl:h-[120px] md:w-14 md:h-12 object-contain opacity-80 hover:opacity-100 transition-opacity duration-300 object-contain"
      />
    </div>

    <!-- Decorative Elements - Foreground -->
    <!-- Crown - Top Left -->
    <div class="absolute top-8 md:top-12 left-8 md:left-16 hidden sm:block z-10">
      <img
        :src="bgArtOne"
        alt="Crown decoration"
        class="xl:w-[125px] xl:h-[92px] xs:w-12 xs:h-10 md:w-14 md:h-12 object-contain opacity-80 hover:opacity-100 transition-opacity duration-300"
      />
    </div>

    <!-- Moon - Left Side -->
    <div class="absolute 2xl:top-90 md:top-32 2xl:left-116 md:left-24 hidden sm:block z-10">
      <img
        :src="bgArtTwo"
        alt="Moon decoration"
        class="w-9 h-9 2xl:h-[72px] 2xl:w-[70px] md:w-10 md:h-10 object-contain opacity-80 hover:opacity-100 transition-opacity duration-300"
      />
    </div>

    <!-- Diamond - Left Bottom -->
    <div class="absolute bottom-24 md:bottom-32 left-12 md:left-20 hidden sm:block z-10">
      <img
        :src="bgArtThree"
        alt="Diamond decoration"
        class="w-10 h-10 md:w-11 md:h-11 object-contain opacity-80 hover:opacity-100 transition-opacity duration-300"
      />
    </div>

    <!-- Clover - Top Right -->
    <div class="absolute top-12 md:top-16 right-16 md:right-20 hidden sm:block z-10">
      <img
        :src="bgArtFour"
        alt="Clover decoration"
        class="w-9 h-10 md:w-10 md:h-11 object-contain opacity-80 hover:opacity-100 transition-opacity duration-300"
      />
    </div>

    <!-- Star - Right Side -->
    <div class="absolute top-36 md:top-40 right-12 md:right-16 hidden md:block z-10">
      <img
        :src="bgArtFive"
        alt="Star decoration"
        class="w-12 h-12 md:w-13 md:h-13 object-contain opacity-80 hover:opacity-100 transition-opacity duration-300"
      />
    </div>

    <!-- Paper Plane - Bottom Right -->
    <div class="absolute bottom-20 md:bottom-24 right-20 md:right-24 hidden sm:block z-10">
      <img
        :src="bgArtSix"
        alt="Paper plane decoration"
        class="w-10 h-10 md:w-11 md:h-11 object-contain opacity-80 hover:opacity-100 transition-opacity duration-300"
      />
    </div>

    <!-- Main Content -->
    <div class="max-w-3xl mx-auto text-center z-20 relative">
      <h1 class="text-3xl md:text-4xl lg:text-5xl font-bold text-white mb-6 md:mb-8 tracking-tight font-[Gellix]">
        About me.
      </h1>

      <div class="space-y-4 md:space-y-6 text-gray-300 text-sm md:text-base lg:text-lg leading-relaxed max-w-2xl mx-auto font-[Gellix]">
        <p class="leading-7">
          I have been coding for more than 6 years. I started my journey at 2018.
        </p>
        <p class="leading-7">
          At first, I learned Java, MySQL, HTML, and CSS to build websites.
        </p>
        <p class="leading-7">
          In October 2021, I started learning React.js, and soon Next.js. I fell in love with this technology and I am now using it professionally.
        </p>
        <p class="leading-7">
          In October 2022, I started working with my first SaaS company. It is called eBoto. It is a versatile web-based voting platform that offers secure online elections for any type of organization.
        </p>
      </div>

      <div class="mt-10 md:mt-12">
        <button class="bg-slate-700/80 hover:bg-slate-600/90 backdrop-blur-sm text-white px-6 md:px-8 py-2.5 md:py-3 rounded-lg font-medium transition-all duration-300 transform hover:scale-105 border border-slate-600/50 hover:border-slate-500/50 shadow-lg hover:shadow-xl font-[Gellix]">
          My Resume
          <svg class="inline-block ml-2 w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"/>
          </svg>
        </button>
      </div>
    </div>
  </div>
</template>

  <script>

  //import ContactForm from '@/sections/ContactForm.vue';

  export default {
    components: {

    },
    data() {
      return {

        bgArtOne : new URL('@/assets/bg-art-1.svg', import.meta.url).href,
        bgArtTwo : new URL('@/assets/bg-art-2.svg', import.meta.url).href,
        bgArtThree : new URL('@/assets/bg-art-3.svg', import.meta.url).href,
        bgArtFour : new URL('@/assets/bg-art-4.svg', import.meta.url).href,
        bgArtFive : new URL('@/assets/bg-art-5.svg', import.meta.url).href,
        bgArtSix : new URL('@/assets/bg-art-6.svg', import.meta.url).href,
        bgArtSeven : new URL('@/assets/bg-art-7.svg', import.meta.url).href,


        mobileMenuOpen: false,
      }
  }
  };
  </script>

  <style scoped>
  </style>
