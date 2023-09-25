<script>

import cardsArray from '../card.js'
import AppMainContent from '../components/AppMainContent.vue'

export default {
  // questo é il vs options object
  name: 'AppMain',
  components: {

    AppMainContent,
  },

  data() {
    return {
      cardsArray,
      
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

        <AppMainContent :image="card.thumb" :title="card.series" :cardsArray="cardsArray" :cards="cardsArray.cards" v-for="(card, i) in cardsArray.cards"> </AppMainContent>
        
        

        
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



.col-12>h2 {
  color: #ffffff;
}
</style>

