<template>
  <div id="app">
    <BaseHeader :urbanTastes="urbanTastes"></BaseHeader>
    <TheMain :bannerAdvs="bannerAdvs" :bannerTeam="bannerTeam" :sliderQuotes="sliderQuotes" :logos="logos" :pizzas="pizzas"></TheMain>
  </div>
</template>

<script>
import BaseHeader from "./components/BaseHeader.vue";
import TheMain from "./components/TheMain.vue"

export default {
  name: 'App',
  components: {
    BaseHeader,
    TheMain,
  },
  data(){
    return {
      bannerAdvs: [
        {
          id: 1,
          url: require('/src/assets/img/h3-img-1.jpg')
        },
        {
          id: 2,
          url: require('/src/assets/img/h3-img-2.jpg')
        },
        {
          id: 3,
          url: require('/src/assets/img/h3-img-3.jpg')
        },
        {
          id: 4,
          url: require('/src/assets/img/h3-img-4.jpg')
        }
      ],
      bannerTeam: [
        {
          id: 1,
          url: require('/src/assets/img/h1-team-1a-700x700.jpg')
        },
        {
          id: 2,
          url: require('/src/assets/img/h1-team-2a.jpg')
        },
        {
          id: 3,
          url: require('/src/assets/img/h1-team-4a.jpg')
        },
        {
          id: 4,
          url: require('/src/assets/img/h1-team-3a.jpg')
        }
      ],
      urbanTastes: [
        {
          url: require('/src/assets/img/h3-rev-img-6.png')
        },
        {
          url: require('/src/assets/img/h3-rev-img-4.png')
        },
        {
          url: require('/src/assets/img/h3-rev-img-2.png')
        }
      ],
      sliderQuotes: [
        {
          id: 1,
          text: "FORGET THE TRENDY PIZZA SHOPS, THIS HIDDEN SPOT MAKES THE BEST NEW YORK-STYLE PIZZA SLICE IN NAPLES",
          author: "WASHINGTON POST 2018"
        },
        {
          id: 2,
          text: "ONE OF THE BEST PIZZA DOUGH EVER",
          author: "WASHINGTON POST 2018"
        },
        {
          id: 3,
          text: "LA MIGLIORE PIZZERIA PER AVERE LA VERA ESPERIENZA NEWYORKESE",
          author: "REPUBBLICA 2022"
        }
      ],
      logos: [
        {
          id: 1,
          url: require('/src/assets/img/h1-clients-img-4.png')
        },
        {
          id: 2,
          url: require('/src/assets/img/h1-clients-img-3.png')
        },
        {
          id: 3,
          url: require('/src/assets/img/h1-clients-img-1.png')
        },
        {
          id: 4,
          url: require('/src/assets/img/h1-clients-img-2.png')
        },
        {
          id: 5,
          url: require('/src/assets/img/h1-clients-img-5.png')
        }
      ],
      pizzas: [
        {
          id: 1,
          url: require('/src/assets/img/h3-product-img-1a-100x100.png'),
          name: 'BISMARK',
          price: '$30.00'
        },
        {
          id: 2,
          url: require('/src/assets/img/h3-product-img-2a-150x150.png'),
          name: 'FIORI DI ZUCCA',
          price: '$7.00 - $50.00'
        },
        {
          id: 3,
          url: require('/src/assets/img/h3-product-img-3a-150x150.png'),
          name: 'VALDOSTANA',
          price: '$55.00'
        },
        {
          id: 4,
          url: require('/src/assets/img/h3-product-img-4a-150x150.png'),
          name: 'PIZZA TARTUFATA',
          price: '$45.00'
        },
        {
          id: 5,
          url: require('/src/assets/img/h3-product-img-5a-150x150.png'),
          name: 'FRANCESCANA',
          price: '$25.00'
        },
        {
          id: 6,
          url: require('/src/assets/img/h3-product-img-6a-100x100.png'),
          name: 'CAMPAGNOLA',
          price: '$50.00 - $95.00'
        }
      ]
    }
  }
  
}
</script>

<style lang="scss">
@import '~bootstrap/scss/bootstrap';
*{
  font-family: 'Roboto Mono', monospace;
}

ul{
  list-style-type: none;
  margin: 0;
  padding: 0;
}

a{
  text-decoration: none;
  color: white;
}

</style>
