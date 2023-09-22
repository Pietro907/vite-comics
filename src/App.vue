<script>
//import HelloWorld from './components/HelloWorld.vue'
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppJumbotron from './components/AppJumbotron.vue'
import AppFooter1 from './components/AppFooter1.vue'
import AppFooter2 from './components/AppFooter2.vue'




export default {
  // questo é il vs options object
  data(){
    return{
      


    }

  },
  components: {
    AppHeader,
    AppMain,
    AppJumbotron,
    AppFooter1,
    AppFooter2,
  }
}

</script>

<template>

  <AppHeader></AppHeader>
  <AppMain></AppMain>
  <AppJumbotron></AppJumbotron>
  <AppFooter1></AppFooter1>
  <AppFooter2></AppFooter2>



</template>

<style>

</style>
