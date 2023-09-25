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
      <div class="row jst_ctr w_jumbo">
  
        <div v-for="link in navJumbo" class="col-3 mx-2 d-flex justify-content-center">
          
          <img :src="link.image" class="image" alt="">
          
          <div class="card">
            <h4>{{ link.text }}</h4>
          </div>
          
        </div>
  
      </div>
    </div>

  </div>

</template>


<style lang="scss">



.container_main {
  background-color: black;
  max-width: 1920px;
  font-family: Arial, Helvetica, sans-serif;
}
.container_content, .jumbotron > .row {
  margin: 0 auto;
}
.container_content {
  width: 70%;
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

.w_jumbo {
  width: 70%;
}
.col-3 {
  
  display: flex;
  align-items: center;
  padding:2rem 1rem;
}
.image {
  width: 60px;
  height: 60px;
  aspect-ratio: 1 / 1;
  object-fit: contain;
}

/* space */

.ms {
  margin-left: 1rem;
}
.card {
  
  width: 135px;
}

/* color */

.bg_black {
  background-color: black;
}



</style>

