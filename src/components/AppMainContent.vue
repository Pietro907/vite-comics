
<script>

export default {
    name: 'AppMainContent',
    props: ['image', 'title', 'cardsArray', 'cards', 'card']
}

</script>



<template>

    <div class="col-2">
        
        <div class="card">
            <img class="img_book" :src="image" :alt="title">

            <h6>{{ title }}</h6>
        </div>

    </div>
    
</template>

<style lang="scss" scoped>


.col-2 {
  color: #ffffff;
  padding: 0.5rem 0.5rem;
  margin: 0 2px;
}

.card>.img_book {
  width: 150px;
  aspect-ratio: 1 / 1;
}

.card {
  width: 150px;
}


</style>