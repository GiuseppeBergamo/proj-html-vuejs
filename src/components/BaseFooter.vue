<template>
  <footer>
    <SplitSectionSecond :items="pizzaDeals" title="DELISH PIZZA DEALS" smallTitle="MADE WITH LOVE"></SplitSectionSecond>
  </footer>
</template>

<script>
import SplitSectionSecond from './SplitSectionSecond.vue';
export default {
    name: 'BaseFooter',
    components: {
        SplitSectionSecond,
    },
    props: {
        pizzaDeals: Array
    }
}
</script>

<style scoped>

</style>