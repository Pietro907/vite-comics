<script>

export default {
  // questo é il vs options object
  name: 'AppMain',
  data() {
    return {
      navMain: [
        {
          title: 'digital comics',
          list:  ['characters','comic','movies','tv','games','videos','news'], 
        },
        {
          title: 'shop',
          list:  ['shop dc','shop dc collectibles'], 
        },
        {
          title: 'dc',
          list:  ['terms of use','privacy','policity (new)','ad choices','adversting','jobs','subscriction','talent','workshops','cpsc','certificates','ratings', 'shop help','contact us'], 
        },
        {
          title: 'sites',
          list:  ['mad','magazine','dc kids','dc univers','dc power visa'], 
        },
        
      ]
    }

  },

}

</script>


<template>
  <main>
    <div class="container container_img">

      <div class="row">

        <div class="col-2">
          <ul class="list_unstyle">
            <li class="title">site</li>
            <li><a href="#">CHARACTERS</a></li>
            
          </ul>

          <ul class="list_unstyle">
            <li class="title">SHOP</li>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
        </div>

        <div class="col-2">
          <ul class="list_unstyle">
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

        </div>

      </div>

      <div class="sing_up">
        <button type="button">SING-UP NOW!</button>
      </div>

    </div>

  </main>
</template>


<style lang="scss">
.container_img {
  background-image: url(.././src/assets/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  flex-direction: column;
}
.container_img > .row {
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

ul > li > a {
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
.sing_up{
  background-color: #000000;
}
</style>

