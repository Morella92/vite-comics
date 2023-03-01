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
  <div class="container body-bg"> 
    
  </div>
  
  <AppHeader/>
  <AppMain/>
  <AppFooter/>
</template>

<style lang="scss" scoped>
@use './style/general.scss';
@use './style/partials/reset';
.body-bg{
    background-color: black;
    min-height: 350px;
}
</style>
