<script>
//import HelloWorld from './components/HelloWorld.vue'
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppJumbotron from './components/AppJumbotron.vue'
import AppFooterp from './components/AppFooterp.vue'
import AppFooterparte from './components/AppFooterparte.vue'




export default {
  // questo é il vs options object
    name: 'App',
  data(){
    return{
      


    }

  },
  components: {
    AppHeader,
    AppMain,
    AppJumbotron,
    AppFooterp,
    AppFooterparte,
  }
}

</script>

<template>

  <AppHeader></AppHeader>
  <AppMain></AppMain>
  <AppJumbotron></AppJumbotron>
  <AppFooterp></AppFooterp>
  <AppFooterparte></AppFooterparte>



</template>

<style>




</style>
