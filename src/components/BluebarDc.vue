<template>
  <div class="icons flex">
    <div class="container flex" v-for="(icon, index) in arrIcons" :key="index">
      <img :src="require('../assets/img/' + icon.img)" :alt="icon.text">
      <span>{{ icon.text }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BluebarDc',
  data () {
    return {
      arrIcons: [
        {
          img: 'buy-comics-digital-comics.png',
          text: 'digital comics'
        },
        {
          img: 'buy-comics-merchandise.png',
          text: 'dc merchandise'
        },
        {
          img: 'buy-comics-subscriptions.png',
          text: 'subscription'
        },
        {
          img: 'buy-comics-shop-locator.png',
          text: 'comic shop locator'
        },
        {
          img: 'buy-dc-power-visa.svg',
          text: 'dc power visa'
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/variables.scss';
.icons{
  padding: 1rem;
  background-color: $blue-dc-color;
  color: white;
  text-transform: uppercase;
  .container{
  align-items: center;
    img{
      // width: 100px;
    }
    span{
      padding-left: 1rem;
    }
  }
}
</style>
