<template>
  <footer>
    <SplitSectionSecond :items="pizzaDeals" title="DELISH PIZZA DEALS" smallTitle="MADE WITH LOVE"></SplitSectionSecond>
    <FormSection :placeholder="placeholder"></FormSection>
  </footer>
</template>

<script>
import SplitSectionSecond from './SplitSectionSecond.vue';
import FormSection from './FormSection.vue';
export default {
    name: 'BaseFooter',
    components: {
        SplitSectionSecond,
        FormSection,
    },
    props: {
        pizzaDeals: Array
    },
    data(){
        return {
            placeholder: '1 Persona'
        }
    }
}
</script>

<style scoped>

</style>