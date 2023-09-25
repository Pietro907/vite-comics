<script>

import brands from '../footer_link'

export default {
  // questo é il vs options object
  name: 'AppFooter',
  data() {
    return {
      brands,
    }

  },

}

</script>


<template>
  <footer>

    <div class="container container_img">

      <div class="row">

        <div v-for="(menu, i) in brands.navMenu" class="col-2">

          <ul class="list_unstyle">

            <li class="title">{{ menu.title }}</li>
            <li class="gray" v-for="name in menu.list"><a href="#"></a> {{ name.name }}</li>

          </ul>

        </div>

      </div>

      <!-- Logo DC in background -->
      <div class="row r_logo">

        <div class="col-4 logo_col">
          <div class="card img_logo_bg">

          </div>
        </div>
      </div>

      
    </div>
    <!-- Sing up & Follow us -->
    <div class="container_foot">

      <div class="row jst_btwn">

        <!-- Button sing up -->
        <div class="col-6 none_bg_img jst_ctr">

          <div class="sing_up">

            <button class="color" type="button">SING-UP NOW!</button>

          </div>

        </div>

        <!-- Follow us and icon brands -->
        <div class="col-6 none_bg_img jst_ctr">

          <div class="features jst_ctr">

            <a href="#"><b>FOLLOW US</b></a>

            <div v-for="pic in brands.brands" class="logo">

              <img :src="pic.logo" :alt="pic.name">

            </div>

          </div>
        </div>
      </div>

    </div>


  </footer>
</template>


<style lang="scss" scoped>
footer {
  font-family: Arial, Helvetica, sans-serif;

}

.container_img {
  background-image: url(.././src/assets/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  max-width: 1920px;
  display: flex;
}

.container_img>.row {
  height: 300px;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  flex-direction: column;
  justify-content: start;
}


.title {
  color: white;
  font-size: large;
}

ul>li>a {
  text-decoration: none;
  color: gray;
}

.list_unstyle {
  list-style: none;
  font-size: small;
  text-align: start;
}



.logo_col {
  height: 350px;
}

.img_logo_bg {
  background-image: url(../assets/img/dc-logo-bg.png);
  background-size: cover;
  background-repeat: no-repeat;
  aspect-ratio: 1 / 1;
  object-fit: cover;
  margin-top: -15px;
}

.r_logo>.col-4 {
  display: flex;
  justify-content: end;
}

.gray {
  color: gray;
}






.container_foot {
  background-color: #303030;
  padding: 2rem 0;
  margin-top: -1rem;

}
.container_foot > .row {
  width: 70%;
  margin: 0 auto;
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

.features {
  margin-left: 3rem;
}

.features>a {
  text-decoration: none;
  color: #0282f9;
  font-size: small;
  padding-right: 1rem;
}

.logo>img {
  width: 25px;
  padding-right: 0.5rem;
}

.color {
  background-color: #303030;
  color: white;
  padding: 0.5rem;
  border: 2px solid #0282f9;
}

.none_bg_img {
  background-image: none;
}

.gray {
  color: gray;
}
</style>




