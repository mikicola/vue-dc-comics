<template>
  <div class="card-container">
    <div class="img-container">
    <img :src="cardThumb" :alt="cardSeries">
    </div>
    <h2 class="title-thumb">{{cardSeries}}</h2>
  </div>
</template>

<script>
export default {
  name: 'CardComics',
  props: {
    // interpreta in automatico (in html è scritto con i - )
    cardThumb: String, // IMMAGINE
    cardSeries: String
  }
}
</script>

<style  scoped lang="scss">
.card-container{
  padding: 2rem 1rem;
}
.img-container {
    width: 200px;
    height: 200px;
    overflow: hidden;
    img {
      background-repeat: no-repeat;
      background-size: auto;
      width: 100%;
    }
  }
  // .img-comics{
  //   object-fit: cover;
  //   width: 100px;
  //   height: 100px;
  // }
  .title-thumb{
    font-size: 1rem;
    font-weight: 200;
    margin-top: 1rem;
  }
</style>
