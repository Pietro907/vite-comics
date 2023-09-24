<script>

export default {
  // questo é il vs options object
  name: 'AppJumbotron',

  data() {
    return {
      navJumbo: [
        {
          text: 'digital comics',
          image:  'src/assets/img/buy-comics-digital-comics.png', 
        },
        {
          text: 'dc merchandise',
          image:  'src/assets/img/buy-comics-merchandise.png', 
        },
        {
          text: 'subscription',
          image:  'src/assets/img/buy-comics-shop-locator.png', 
        },
        {
          text: 'comic shop locator',
          image:  'src/assets/img/buy-comics-subscriptions.png', 
        },
        {
          text: 'dc power visa',
          image:  'src/assets/img/buy-dc-power-visa.svg', 
        },        
      ]
    }

  },

}

</script>


<template>
  <div class="container_main">

    <!-- Content goes here -->
    <div class="container_content">
      <div class="row r_container">
        <div class="col-12">
          <h2 class="ms"> Content goes here </h2>
        </div>
      </div>
    </div>
  
    <!-- jumbotron -->
    <div class="jumbotron">
      <div class="row">
  
        <div v-for="link in navJumbo" class="col-5 mx-2 d-flex justify-content-center">
          
          <img :src="link.image" class="image" alt="">
          
          <div class="card">
            {{ link.text }}
          </div>
          
        </div>
  
      </div>
    </div>

  </div>

</template>


<style lang="scss">

.container_main {
  background-color: black;
}
.container_content {
  width: 70%;
  margin: 0 auto;
}

.col-12 {
  height: 200px;
  display: flex;
  align-items: center;
}

.col-12 > h2 {
  color: #ffffff;
}
.jumbotron {
  background-color: #0282f9;
}
.r_jumbo {
  display: flex;
  flex-direction: row;
  justify-content: space-between;

}
.col-5 {
  height: 200px;
  display: flex;
  align-items: center;
  padding:2rem 1rem;
}
.image {
  width: 60px;
  height: 70px;
  aspect-ratio: 1 / 1;
}

/* space */

.ms {
  margin-left: 1rem;
}


/* color */

.bg_black {
  background-color: black;
}



</style>

