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
    <div class="container_header">
      <div class="row jst_btwn">
        <div class="col-3">

          <!-- Logo immagine -->
          <img src="../assets/img/dc-logo.png" alt="logo DC Univers">

        </div>

        <div class="col-9 ">

          <!-- Navbar header loop per 10 -->
          <nav class="navbar navbar-expand-sm jst_btwn">
            <div v-for="linkHeader in navHeader" class="container_a pad_x">
      
              <a class="navbar-brand text-red text-uppercase" href="#">{{ linkHeader }}</a>
              
            </div>
          </nav>

        </div>
      </div>

  

  

    </div>


  </header>



</template>


<style lang="scss" scoped>

header {
  font-family: Arial, Helvetica, sans-serif;
}

.container_header {
  max-width: 1920px;
}


.container_header > .row {
  width: 70%;
  margin: 0 auto;

}

.container_a > a {
  text-decoration: none;
  color: black;
}

.jst_ctr {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}

.jst_btwn {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}


/* space */

.pad_x {
  padding: 0 0.5rem;
}


/* 
.active {
  background-color: #0282f9;
} */

</style>

