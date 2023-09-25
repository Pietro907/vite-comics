<script>

import jumbo from '../jumbo.js'

export default {
  // questo é il vs options object
  name: 'AppJumbotron',

  data() {
    return {
      jumbo,
    }
  },

}

</script>


<template>
  
 
  
  
    <!-- jumbotron -->
    <div class="jumbotron">
      <div class="row jst_ctr w_jumbo">
  
        <div v-for="(link , i) in jumbo.navJumbo" class="col-3">
          
          <img :src="link.image" class="image" alt="">
          
          <div class="card">
            <h4 class="ms">{{ link.text }}</h4>
          </div>
          
        </div>
  
      </div>
    </div>



</template>


<style lang="scss" scoped>

//@use '../assets/scss/particials/variables' as *;



.jumbotron {
  background-color: #0282f9;
}

.w_jumbo {
  width: 70%;
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;

}
.col-3 {
  width: calc(100% / 12 * 3);
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 1rem 0;
  color: #ffffff;
}
.image {
  width: 40px;
  height: 40px;
  aspect-ratio: 1 / 1;
  object-fit: contain;
}

/* space */

.ms {
  margin-left: 0.5rem;
}
.card {
  
  width: 100%;
}

/* color */

.bg_black {
  background-color: black;
}



</style>

