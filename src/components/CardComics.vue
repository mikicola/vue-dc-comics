<template>
  <div>
    <img :src="cardThumb" :alt="cardSeries">
    <h2>{{cardSeries}}</h2>
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

<style>

</style>
