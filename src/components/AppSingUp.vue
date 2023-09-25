<script>

export default {
  // questo é il vs options object
  name: 'AppSingUp',
  data() {
    return {
    }
  }
}

</script>


<template>

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

            <div v-for="brand in brands" class="logo">

              <img :src="brand.logo" :alt="brand.name">

            </div>

          </div>
        </div>
      </div>

    </div>

</template>


<style lang="scss" scoped>



/* features */


.container_foot {
  background-color: #303030;
  padding: 2rem;
  margin-top: -1rem;
 
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



.features > a {
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

