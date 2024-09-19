<template>
  <navbar></navbar>

</template>

<script>
  import Navbar from './components/Navbar.vue';
  import HeroSection from './components/HeroSection.vue';

  export default{
  components:{
    Navbar,
    HeroSection,
  },
  data() {
    return {
      navItems: [],
      activeNavItem: 0,
      darkNavBar: false,
    }
  },
  methods: {
    async initNavItems(){
      try {
        let res = await fetch('./navItems.json');
        let data = await res.json();

        this.navItems = data;
        console.log(this.navItems)
        console.log(data)
      }catch(err){
        console.log('Something Error', err)
      }
    },
  },
  mounted(){
    this.initNavItems();
  },
}
</script>

<style scoped>
</style>