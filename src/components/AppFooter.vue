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

        <div v-for="menu in brands.navMenu" class="col-2">

          <ul class="list_unstyle">

            <li class="title">{{ menu.title }}</li>
            <li class="gray" v-for="name in menu.list"><a href="#"></a> {{ name.name }}</li>

          </ul>

        </div>

      </div>

      <!-- Logo DC in background -->
      <div class="row r_logo">

        <div class="col-4">
          <div class="card img_logo_bg">
            
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

.container_img > .row {
  width: 70%;
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


.img_logo_bg {
  background-image: url(../assets/img/dc-logo-bg.png);
  background-size: contain;
  background-repeat: no-repeat;
  height: 300px;
  aspect-ratio: 1 / 1;
  object-fit: cover;

}
.r_logo > .col-4 {
  display: flex;
  justify-content: end;
}

.gray {
  color: gray;
}





</style>

