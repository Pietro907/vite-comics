<script>

export default {
  // questo é il vs options object
  name: 'AppFooter',
  data() {
    return {
      brands: [
        {
          name: 'facebook',
          logo: 'src/assets/img/footer-facebook.png',
        },
        {
          name: 'twitter',
          logo: 'src/assets/img/footer-twitter.png',
        },
        {
          name: 'youtube',
          logo: 'src/assets/img/footer-youtube.png',
        },
        {
          name: 'pinterest',
          logo: 'src/assets/img/footer-pinterest.png',
        },
        {
          name: 'periscope',
          logo: 'src/assets/img/footer-periscope.png',
        },
      ],
      navMenu: [
        {
          title: 'digital comics',
          list: [
            {
              name: 'characters'
            },
            {
              name: 'comic'
            },
            {
              name: 'movies'
            },
            {
              name: 'tv'
            },
            {
              name: 'games'
            },
            {
              name: 'videos'
            },
            {
              name: 'news'
            },
          ],
        },
        {
          title: 'shop',
          list: [{ name: 'shop dc' }, { name: 'shop dc collectibles' }],
        },
        {
          title: 'dc',
          list: [
            {
              name: 'terms of use'
            },
            {
              name: 'privacy'
            },
            {
              name: 'policity (new)'
            },
            {
              name: 'ad choices'
            },
            {
              name: 'adversting'
            },
            {
              name: 'jobs'
            },
            {
              name: 'subscriction'
            },
            {
              name: 'talent'
            },
            {
              name: 'workshops'
            },
            {
              name: 'cpsc'
            },
            {
              name: 'certificates'
            },
            {
              name: 'ratings'
            },
            {
              name: 'shop help'
            },
            {
              name: 'contact us'
            },
          ],
        },
        {
          title: 'sites',
          list: ['mad', 'magazine', 'dc kids', 'dc univers', 'dc power visa'],
        },

      ]

    }

  },

}

</script>


<template>
  <footer>
    <div class="container container_img">

      <div class="row">

        <div v-for="menu in navMenu" class="col-2">

          <ul class="list_unstyle">

            <li class="title">{{ menu.title }}</li>
            <li class="gray" v-for="name in menu.list"><a href="#"></a> {{ name.name }}</li>

          </ul>


        </div>
        <!-- <div  class="col-2">

          <ul  class="list_unstyle">

            <li class="title">DC </li>
            <li><a href="#">Terms Of Use</a></li>
            <li><a href="#">Privacy Policity (New)</a></li>
            <li><a href="#">Ad Choices</a></li>
            <li><a href="#">Adversting</a></li>
            <li><a href="#">Jobs</a></li>
            <li><a href="#">Subscriction</a></li>
            <li><a href="#">Talent Workshops</a></li>
            <li><a href="#">CPSC Certificates</a></li>
            <li><a href="#">Ratings</a></li>
            <li><a href="#">Shop Help</a></li>
            <li><a href="#">Contact Us</a></li>

          </ul>

        </div>

        <div class="col-2">

          <ul class="list_unstyle">

            <li class="title">SITES</li>
            <li><a href="#">MAD Magazine</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Univers</a></li>
            <li><a href="#">DC Power Visa</a></li>

          </ul>

        </div>

        <div class="col-6">

        </div> -->

      </div>


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

              <div v-for="brand in brands" class="logo">

                <img :src="brand.logo" :alt="brand.name">

              </div>

            </div>
          </div>
        </div>





      </div>



    </div>

  </footer>
</template>


<style lang="scss">
.container_img {
  background-image: url(.././src/assets/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  flex-direction: column;
  max-width: 1920px;

}

.container_img>.row {
  width: 70%;
  margin: 0 auto;
}

.row {
  display: flex;
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

.col-6 {
  background-image: url(../assets/img/dc-logo-bg.png);
  background-size: contain;
  background-repeat: no-repeat;
  width: 100%;
  margin: -2rem 0 -2rem 2rem;
}


/* features */



footer {
  font-family: Arial, Helvetica, sans-serif;

}

.container_foot {
  background-color: #303030;
  padding: 2rem 0;
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

/* .sing_up {


} */

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

