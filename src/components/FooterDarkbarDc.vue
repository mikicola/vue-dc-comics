<template>
  <div class="footer-bottom">
    <div class="container flex">
      <div class="sign-up"><a href="#">Sign up!</a></div>
      <div>
        follow us
        <ul class="social-icons">
          <li v-for="(socialIcons, index) in arrSocialIcons" :key="index">
            <img :src="require('../assets/img/' + socialIcons.img)" alt="">
          </li>
        </ul>
        </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FooterDarkbarDc',
  data () {
    return {
      arrSocialIcons: [
        {
          img: 'footer-facebook.png'
        },
        {
          img: 'footer-periscope.png'
        },
        {
          img: 'footer-pinterest.png'
        },
        {
          img: 'footer-twitter.png'
        },
        {
          img: 'footer-youtube.png'
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/variables.scss';
.footer-bottom{
  background-color: $navbar-color;
  text-transform: uppercase;
  font-size: 1.5rem;
  .container{
    justify-content: space-between;
  }
}
// $navbar-color
</style>
