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
    <div class="container-fluid">
      <div class="row">
        <div class="col-3">

          <!-- Logo immagine -->
          <img src="../assets/img/dc-logo.png" alt="logo DC Univers">

        </div>

        <div class="col-9 d-flex">
          <!-- Navbar header -->
          <nav class="navbar navbar-expand-sm navbar-dark bg-dark">
            <div class="container-fluid menu_nav">
      
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

        </div>
      </div>

  

  

    </div>


  </header>



</template>


<style lang="scss" scoped>


.row {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.menu_nav {
  background-color: #ffffff;
}
.menu_nav > a {
  padding: 0 0.5rem;
  color: #1c1c1c;
}

.active {
  background-color: #0282f9;
}

</style>

