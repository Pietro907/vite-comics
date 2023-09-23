<script>

export default {
  // questo é il vs options object
  name: 'AppMain',
  data() {
    return {

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
            <li class="title">DC COMICS</li>
            <li><a class="tile" href="#">CHARACTERS</a></li>
            <li><a href="#">COMIC</a></li>
            <li><a href="#">MOVIES</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">GAMES</a></li>
            <li><a href="#">VIDEOS</a></li>
            <li><a href="#">NEWS</a></li>
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

