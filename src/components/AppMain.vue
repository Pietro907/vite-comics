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

        <div v-for="item in cards" class="col-6">
          <img src="../assets/img/buy-comics-merchandise.png" alt="">
          <h2>{{item.price}}</h2>
          <h2>series</h2>
          <h2>type</h2>
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

.col-6 {
  color: #ffffff;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 0.5rem 0;
}

.col-12>h2 {
  color: #ffffff;
}
</style>

