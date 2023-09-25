<script>

import cards from '../card.js'

export default {
  // questo é il vs options object
  name: 'AppMain',


  data() {
    return {
      cards,
      props: {
        img: String,
        big: String,
        small: String,
      }
    }
  },
}

</script>


<template>
  <div class="current_series"><b>CURRENT SERIES</b></div>
  <section>

    <div class="content img_jumbo">






    </div>

  </section>
  <div class="container_main">

    <!-- Content goes here -->
    <div class="container_content">

      <div class="row">

        <div v-for="(card, i) in cards.cards" class="col-2">
          <!-- <h2>{{card.price}}</h2> -->
          <div class="card">
            <img class="img_book" :src="img" :alt="small">

            <h6>{{ card.series }}</h6>
          </div>
          <!-- <h2>{{card.type}}</h2> -->
        </div>
      </div>

    </div>

    <div class="container_foot">
  
      <div class="row jst_btwn">
  
        <!-- Button load more -->
        <div class="col none_bg_img jst_ctr">
  
          <div class="sing_up">
  
            <button class="color" type="button"><b>LOAD MORE</b></button>
  
          </div>
  
        </div>
  
      </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.current_series {
  background-color: #0282f9;
  padding: 0.5rem;
  color: #ffffff;
  position: absolute;
  top: 390px;
  left: 180px;
}
.container_foot{
  display: flex;
  justify-content: center;
}
.color {
  background-color: #0282f9;
  color: #ffffff;
  padding: 0.5rem 3rem;
  margin: -1.5rem 0 1.5rem;
  border: none;
}
main {
  font-family: Arial, Helvetica, sans-serif;

}

.content {
  margin-bottom: -1rem;
}

.img_jumbo {
  background-image: url('../assets/img/jumbotron.jpg');
  background-size: cover;
  width: 100%;
  height: 350px;


}

.container_main {
  background-color: black;
  max-width: 1920px;
  font-family: Arial, Helvetica, sans-serif;
}

.container_content {
  width: 70%;
  margin: 0 auto;
}

.row {
  display: flex;
  flex-wrap: wrap;
  padding: 1rem 0 0;
}

.col-2 {
  color: #ffffff;
  padding: 0.5rem 0.5rem;
  margin: 0 2px;
}

.card>.img_book {
  width: 150px;
  aspect-ratio: 1 / 1;
}

.card {
  width: 150px;
}

.col-12>h2 {
  color: #ffffff;
}
</style>

