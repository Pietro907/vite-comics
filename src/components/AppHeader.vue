<script>

export default {
  // questo é il vs options object
  name: 'AppHeader',


  data(){
    return{
        
    
    }

  },
 
}

</script>


<template>

  <header>
    <!-- Logo immagine -->
    <div class="logo">

      <img src="../assets/img/dc-logo.png" alt="logo DC Univers">

    </div>

    <!-- Navbar header -->
    <nav class="navbar fixed-bottom navbar-expand-sm navbar-dark bg-dark">
      <div class="container-fluid">

        <a class="navbar-brand" href="#">CHARACTERS</a>
        <a class="navbar-brand" href="#">COMIC</a>
        <a class="navbar-brand" href="#">MOVIES</a>
        <a class="navbar-brand" href="#">TV</a>
        <a class="navbar-brand" href="#">GAMES</a>
        <a class="navbar-brand" href="#">COLLECTIBLES</a>
        <a class="navbar-brand" href="#">VIDEOS</a>
        <a class="navbar-brand" href="#">FANS</a>
        <a class="navbar-brand" href="#">NEWS</a>
        <a class="navbar-brand" href="#">SHOP</a>

      </div>
    </nav>


  </header>



</template>


<style lang="scss" scoped>

.container-fluid > a {
  padding: 0 0.5rem;
}


</style>

