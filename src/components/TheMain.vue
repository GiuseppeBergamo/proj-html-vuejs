<template>
  <main>
    <BannerSection :items="bannerAdvs" class="mb-2"></BannerSection>
    <section id="slider-section" class="mb-2">
        <BaseSlider :items="sliderQuotes"></BaseSlider>
    </section>
    <SplitSectionFirst></SplitSectionFirst>
    <BaseJumbotron></BaseJumbotron>
    <BannerSection :items="bannerTeam" class="mb-2"></BannerSection>
    <LogosSection :items="logos"></LogosSection>
  </main>
</template>

<script>
import BannerSection from "./BannerSection.vue";
import BaseSlider from "./BaseSlider.vue";
import SplitSectionFirst from "./SplitSectionFirst.vue";
import BaseJumbotron from "./BaseJumbotron.vue"
import LogosSection from "./LogosSection.vue";
export default {
    name: 'TheMain',
    components: {
    BannerSection,
    BaseSlider,
    SplitSectionFirst,
    BaseJumbotron,
    LogosSection
},
    props: {
        bannerAdvs: Array,
        bannerTeam: Array,
        sliderQuotes: Array,
        logos: Array
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