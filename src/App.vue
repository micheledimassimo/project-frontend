<script>

import AppHeader from './components/AppHeader.vue';
import AppBiography from './components/AppBiography.vue';

export default {
  data() {
    return { 
      
    }
  },
 
  components: {
    AppHeader,
    AppBiography
  },
  methods: {
    
  }
}
</script>

<template>
  <div>
   
    <AppHeader />
    
    <AppBiography />
  </div>
</template>

<style lang="scss">
@use 'assets/scss/main' as *;
// Import all of Bootstrap's CSS
@import "bootstrap/scss/bootstrap";
</style>
