<template>
  <div id="app">
    <BaseHeader></BaseHeader>
    <TheMain :bannerAdvs="bannerAdvs" :bannerTeam="bannerTeam"></TheMain>
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
          url: require('/src/assets/img/h1-team-3a.jpg')
        },
        {
          id: 4,
          url: require('/src/assets/img/h1-team-2a.jpg')
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
