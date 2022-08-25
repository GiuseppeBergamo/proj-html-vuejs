<template>
  <footer>
    <SplitSectionSecond :items="pizzaDeals" title="DELISH PIZZA DEALS" smallTitle="MADE WITH LOVE"></SplitSectionSecond>
    <FormSection :placeholder="placeholder"></FormSection>
    <SplitSectionThird :items="workingHours" title="WORKING HOURS"></SplitSectionThird>
  </footer>
</template>

<script>
import SplitSectionSecond from './SplitSectionSecond.vue';
import FormSection from './FormSection.vue';
import SplitSectionThird from './SplitSectionThird.vue'
export default {
    name: 'BaseFooter',
    components: {
        SplitSectionSecond,
        FormSection,
        SplitSectionThird,
    },
    props: {
        pizzaDeals: Array,
        workingHours: Array
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