<script>

export default {
  // questo é il vs options object
  name: 'AppJumbotron',

  data() {
    return {
      navJumbo: [
        {
          text: 'digital comics',
          image:  './src/assets/img/buy-comics-digital-comics.png', 
        },
        {
          text: 'dc merchandise',
          image:  './src/assets/img/buy-comics-merchandise.png', 
        },
        {
          text: 'subscription',
          image:  './src/assets/img/buy-comics-shop-locator.png', 
        },
        {
          text: 'comic shop locator',
          image:  './src/assets/img/buy-comics-subscriptions.png', 
        },
        {
          text: 'dc power visa',
          image:  './src/assets/img/buy-dc-power-visa.png', 
        },
        
      ]
    }

  },

}

</script>


<template>

  <!-- Content goes here -->
  <div class="container">
    <div class="row r_container">
      <div class="col-12">
        <h2> Content goes here </h2>
      </div>
    </div>
  </div>

  <!-- jumbotron -->
  <div class="jumbotron">
    <div class="row r_jumbo">

      <div v-for="link in navJumbo" class="col">
        
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
        
        <div class="card">
        
        </div>
      </div>

      <!-- <div class="col">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
      </div>

      <div class="col">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
      </div>

      <div class="col">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
      </div>

      <div class="col">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
      </div>
 -->
    </div>
  </div>
</template>


<style lang="scss">


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
.col {
  height: 200px;
  display: flex;
  align-items: center;
  padding: 3rem;
}
.col > img {
  width: 70px;
}


</style>

