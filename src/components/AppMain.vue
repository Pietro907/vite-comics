<script>

import cards from '../card.js'

export default {
  // questo é il vs options object
  name: 'AppMain',

  
  data() {
    return {
      cards,
    }

  },

}

</script>


<template>
  <div class="container_main">

    <!-- Content goes here -->
    <div class="container_content">

      <div class="row">

        <div v-for="(card, i) in cards.cards" class="col-2">
          <!-- <h2>{{card.price}}</h2> -->
          <div class="card">
            <img :src="card.thumb" alt="">

            <h6>{{card.series}}</h6>
          </div>
          <!-- <h2>{{card.type}}</h2> -->
        </div>
      </div>

    </div>

  </div>
</template>


<style lang="scss" scoped>
main {
  font-family: Arial, Helvetica, sans-serif;

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
  margin: 0 5px;
}
.card> img {
  width: 110px;
  aspect-ratio: 1 / 1;
}
.card {
  width: 100px;
}
.col-12>h2 {
  color: #ffffff;
}
</style>

