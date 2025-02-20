<script>

import AppHeader from './components/AppHeader.vue';
import AppBiography from './components/AppBiography.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  data() {
    return { 
      
    }
  },
 
  components: {
    AppHeader,
    AppBiography,
    AppMain,
    AppFooter
  },
  methods: {
    
  }
}
</script>

<template>
  <div>
   
    <AppHeader />
    
    <AppBiography />

    <AppMain />

    <AppFooter />
  </div>
</template>

<style lang="scss">
@use 'assets/scss/main' as *;
// Import all of Bootstrap's CSS
@import "bootstrap/scss/bootstrap";
</style>
