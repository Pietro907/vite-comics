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
  <div class="container_main">

    <!-- Content goes here -->
    <div class="container_content">

      <div class="row r_container">
        <div class="col-12">
          <h2 class=""> Content goes here </h2>
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

.col-12 {
  height: 100px;
  display: flex;
  align-items: center;
  padding: 0.5rem 0;
}

.col-12 > h2 {
  color: #ffffff;
}
</style>

