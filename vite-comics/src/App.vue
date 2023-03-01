<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppFooter,
    AppHeader,
    AppMain,
  }
}
</script>

<template>
  <div class="container"> 
    ciao
  </div>
  
  <AppHeader/>
  <AppMain/>
  <AppFooter/>
</template>

<style lang="scss" scoped>
@use './style/general.scss';
@use './style/partials/reset';
</style>
