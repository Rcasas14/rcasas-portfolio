<template>
  <navbar :nav-items="navItems"  ></navbar>

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
      
      darkNavBar: false,
    }
  },
  methods: {
    initNavItems(){
      try {
        // let res = await fetch('./navItems.json');
        // let data = await res.json();
        const navItems = [
          { key: "home", text: "Home", url: "#home" },
          { key: "project", text: "Project", url: "#project" },
        ];

        const mainNav = navItems.map((item)=>{
          return item
        });
        
        this.navItems = mainNav;
        console.log(mainNav)
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