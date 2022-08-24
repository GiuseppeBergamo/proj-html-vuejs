<template>
  <div id="app">
    <BaseHeader></BaseHeader>
  </div>
</template>

<script>
import BaseHeader from "./components/BaseHeader.vue";


export default {
  name: 'App',
  components: {
    BaseHeader,
  },
  
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
