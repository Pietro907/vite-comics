<script>

export default {
  // questo é il vs options object
  name: 'AppHeader',


  data(){
    return{
      navHeader: ['characters', 'comics', 'movies', 'tv', 'games', 'collectibles', 'videos', 'fans', 'news', 'shop']
    
    }

  },
 
}

</script>


<template>

  <header>
    <div class="container">
      <div class="row">
        <div class="col-3">

          <!-- Logo immagine -->
          <img src="../assets/img/dc-logo.png" alt="logo DC Univers">

        </div>

        <div class="col-9 jst_ctr">

          <!-- Navbar header loop per 10 -->
          <nav class="navbar navbar-expand-sm">
            <div v-for="linkHeader in navHeader" class="container">
      
              <a class="navbar-brand text-red text-uppercase" href="#">{{ linkHeader }}</a>
              
            </div>
          </nav>

        </div>
      </div>

  

  

    </div>


  </header>



</template>


<style lang="scss" scoped>

.jst_ctr {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}


/* 
.active {
  background-color: #0282f9;
} */

</style>

