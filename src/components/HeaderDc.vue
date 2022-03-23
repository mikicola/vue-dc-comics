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

.header {
  display: flex;
  justify-content: space-between;
}
  li{
    display: inline-block;
    text-transform: uppercase;
    a{
      text-decoration: none;
      color: navbar;
    }
  }
</style>
