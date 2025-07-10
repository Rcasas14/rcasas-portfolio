<template>
  <transition name="slide-up" @after-leave="onTransitioned">
    <div v-if="loading" class="loading-screen" >
      <div class="h-full flex flex-col justify-center items-center">
      </div>
    </div>
  </transition>
</template>

<script>
export default {
setup(){


    },
  data() {
    return {
      loading: true
    }
  },
  mounted() {
    setTimeout(() => {
      this.loading = false
      console.log('Loading Completed: ', this.loading)
    }, 1300)
  },
  methods: {
    onTransitioned() {
      console.log('Transition completed, component removed')
      this.$emit('loading-complete')
    }
  }
}
</script>

<style scoped>

.loading-screen {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: white; /* Or your hero-bg color */
  z-index: 9999;
}

/* Vue transition classes */
.slide-up-leave-active {
  transition: transform 0.3s ease-in-out;
}

.slide-up-leave-to {
  transform: translateY(-100%);
}

</style>
