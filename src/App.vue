<script>
//import HelloWorld from './components/HelloWorld.vue'
import AppHeader from './components/AppHeader.vue'
import AppJumbotron from './components/AppJumbotron.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'





export default {
  // questo é il vs options object
    
  data(){
    return{
      


    }

  },
  components: {
    AppHeader,
    AppJumbotron,
    AppMain,
    AppFooter,
    
  }
}

</script>

<template>

  <AppHeader></AppHeader>

  <AppJumbotron></AppJumbotron>

  <AppMain></AppMain>

  <AppFooter></AppFooter>



</template>

<style lang="scss" scope>

  //@use './assets/scss/particials/variables.scss' as *
 

</style>
