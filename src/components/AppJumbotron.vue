<script>

export default {
  // questo é il vs options object
  name: 'AppJumbotron',

  data() {
    return {

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

      <div class="col">
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

      <div class="col">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
      </div>

    </div>
  </div>
</template>


<style lang="scss">

.container{
  background-color: #1c1c1c;
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

