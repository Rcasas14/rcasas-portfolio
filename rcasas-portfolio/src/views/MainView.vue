<template>
    <!-- <navbar-component v-if="!loading" />

      <loading-component v-if="loading" />
      <router-view v-if="!loading" />

    <footer-component v-if="!loading" class="absolute bottom-0 w-full" /> -->
    <navbar-component />
      <router-view></router-view>

    <footer-component class="absolute bottom-0 w-full" />
</template>

<script>
import NavbarComponent from '../components/NavbarComponent.vue';
// import LoadingComponent from '@/components/LoadingComponent.vue';
import FooterComponent from '@/components/FooterComponent.vue';
export default {
  components: {
    NavbarComponent,
    // LoadingComponent,
    FooterComponent
  },
  data() {
    // return {
    //   loading: true,
    // };
  },
  // mounted(){
  //   setTimeout(()=>{
  //     this.loading = false
  //     console.log('Loading Completed: ', this.loading)
  //   }, 1300)
  // }
};
</script>

<style scoped></style>
