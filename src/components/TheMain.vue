<template>
  <main>
    <BannerSection :items="bannerAdvs" class="mb-2"></BannerSection>
    <section id="slider-section" class="mb-2">
        <BaseSlider :items="sliderQuotes"></BaseSlider>
    </section>
  </main>
</template>

<script>
import BannerSection from "./BannerSection.vue"
import BaseSlider from "./BaseSlider.vue"
export default {
    name: 'TheMain',
    components: {
        BannerSection,
        BaseSlider
    },
    props: {
        bannerAdvs: Array,
        bannerTeam: Array,
        sliderQuotes: Array
    }
}
</script>

<style scoped>
#slider-section{
    background-image: url('../assets/img/h3-testimonials-bckgrnd.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
}
</style>