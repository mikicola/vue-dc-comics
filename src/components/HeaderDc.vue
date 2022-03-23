<template>
  <header>
    <div class="header container">
      <img src="../assets/img/dc-logo.png" alt="">
      <ul>
        <li v-for="(link, index)  in navbarLinks" :key="index"><a :href="link.href">{{link.text}}</a></li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderDc',
  data () {
    return {
      navbarLinks: [
        {
          text: 'Characters',
          href: '#'
        },
        {
          text: 'Comics',
          href: '#'
        },
        {
          text: 'Movies',
          href: '#'
        },
        {
          text: 'tv',
          href: '#'
        },
        {
          text: 'games',
          href: '#'
        },
        {
          text: 'Collectibles',
          href: '#'
        },
        {
          text: 'videos',
          href: '#'
        },
        {
          text: 'fans',
          href: '#'
        },
        {
          text: 'news',
          href: '#'
        },
        {
          text: 'Shop',
          href: '#'
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/variables.scss';
header{
  background-color: aquamarine;
}

.header {
  display: flex;
  justify-content: space-between;
}

img {
  display: block;
  height: 4rem;
  width: 4rem;
  margin: 1rem 0;
}
  li{
    display: inline-block;
    text-transform: uppercase;
    height: 100%;
    a{
      text-decoration: none;
      color: $navbar-color;
      margin-left: 1rem;
      font-weight: 700;
      height: 100%;
      display: flex;
      align-items: center;
      border-bottom: 0.4rem transparent solid;
      &:hover {
            border-bottom: 0.4rem $blue-dc-color solid;
            color: $blue-dc-color;
          }
    }
  }
</style>
