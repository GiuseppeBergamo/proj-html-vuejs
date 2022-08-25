<template>
  <section id="banner" class="d-flex">
    <div class="row row-cols-4 g-0">
        <BannerCard v-for="item in items" :key="item.id" :card="item"></BannerCard>
    </div>
  </section>
</template>

<script>
import BannerCard from './BannerCard.vue';
export default {
    name: "BannerSection",
    props: {
        items: Array,
    },
    components: { BannerCard }
}
</script>

<style scoped>
#banner {
  min-height: 100px;
}
</style>