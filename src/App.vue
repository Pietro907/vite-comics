<script>
//import HelloWorld from './components/HelloWorld.vue'
import AppHeader from './components/AppHeader.vue'
import AppJumbotron from './components/AppJumbotron.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
import AppSingUp from './components/AppSingUp.vue'




export default {
  // questo é il vs options object
    name: 'App',
  data(){
    return{
      


    }

  },
  components: {
    AppHeader,
    AppJumbotron,
    AppMain,
    AppFooter,
    AppSingUp,
    
  }
}

</script>

<template>

  <AppHeader></AppHeader>
  
  <AppMain></AppMain>
  <AppJumbotron></AppJumbotron>


  <AppFooter></AppFooter>
  <AppSingUp></AppSingUp>


</template>

<style lang="scss" scope>

  //@use './assets/scss/particials/variables.scss' as *


</style>
