<template>
  <footer>
    <div class="container">
      <ul class="dc-comics">
        <li class="title">dc comics</li>
        <li v-for="(dccomics, index) in arrDcComics" :key="index">{{ dccomics.text }}<a :href="dccomics.link"></a> </li>
      </ul>
      <ul class="shop">
        <li class="title">shop</li>
        <li v-for="(shop, index) in arrShop" :key="index">
          {{ shop.text }}
          <a :href="shop.link"></a>
          </li>
      </ul>
      <ul class="dc">
        <li class="title">dc</li>
        <li v-for="(dc, index) in arrDc" :key="index">
          {{ dc.text }}
          <a :href="dc.link"></a>
          </li>
      </ul>
      <ul class="sites">
        <li class="title">sites</li>
        <li v-for="(sites, index) in arrSites" :key="index">
          {{ sites.text }}
          <a :href="sites.link"></a>
          </li>
      </ul>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterDc',
  data () {
    return {
      arrDcComics: [
        {
          link: '#',
          text: 'testo1'
        },
        {
          link: '#',
          text: 'testo2'
        },
        {
          link: '#',
          text: 'testo3'
        },
        {
          link: '#',
          text: 'testo4'
        },
        {
          link: '#',
          text: 'testo'
        },
        {
          link: '#',
          text: 'testo'
        },
        {
          link: '#',
          text: 'testo'
        }

      ],
      arrShop: [
        {
          link: '#',
          text: 'testo1'
        },
        {
          link: '#',
          text: 'testo2'
        }
      ],
      arrDc: [
        {
          link: '#',
          text: 'testo1'
        },
        {
          link: '#',
          text: 'testo2'
        },
        {
          link: '#',
          text: 'testo3'
        },
        {
          link: '#',
          text: 'testo4'
        },
        {
          link: '#',
          text: 'testo'
        },
        {
          link: '#',
          text: 'testo'
        },
        {
          link: '#',
          text: 'testo'
        },
        {
          link: '#',
          text: 'testo'
        },
        {
          link: '#',
          text: 'testo'
        },
        {
          link: '#',
          text: 'testo'
        },
        {
          link: '#',
          text: 'testo'
        }
      ],
      arrSites: [
        {
          link: '#',
          text: 'testo1'
        },
        {
          link: '#',
          text: 'testo2'
        },
        {
          link: '#',
          text: 'testo3'
        },
        {
          link: '#',
          text: 'testo4'
        },
        {
          link: '#',
          text: 'testo'
        },
        {
          link: '#',
          text: 'testo'
        },
        {
          link: '#',
          text: 'testo'
        },
        {
          link: '#',
          text: 'testo'
        },
        {
          link: '#',
          text: 'testo'
        },
        {
          link: '#',
          text: 'testo'
        },
        {
          link: '#',
          text: 'testo'
        }
      ]

    }
  }
}
</script>

<style scoped lang="scss">
@import '../assets/styles/partials/variables.scss';
footer{
  color: white;
  .title{
    text-transform: uppercase;
  }
}
</style>
