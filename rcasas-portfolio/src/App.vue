<template>
  <navbar></navbar>

</template>

<script>
  import Navbar from './components/Navbar.vue';

  export default{
  components:{
    Navbar,
  },
  data() {
    return {
      name: 'WORLD',
    }
  }
}
</script>

<style scoped>
</style>