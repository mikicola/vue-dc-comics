<template>
  <div id="app">
    <HeaderDc />
    <MainDc />
    <BluebarDc />
    <FooterDc />
    <FooterDarkbarDc />
  </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue'
import MainDc from './components/MainDc.vue'
import BluebarDc from './components/BluebarDc.vue'
import FooterDc from './components/FooterDc.vue'
import FooterDarkbarDc from './components/FooterDarkbarDc.vue'

export default {
  name: 'App',
  components: {
    HeaderDc,
    MainDc,
    BluebarDc,
    FooterDc,
    FooterDarkbarDc
  }
}
</script>

<style lang="scss">
@import "./assets/styles/style.scss";

</style>
