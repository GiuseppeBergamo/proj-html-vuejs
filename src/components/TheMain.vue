<template>
  <BannerSection :items="bannerAdvs" class="mb-2"></BannerSection>
</template>

<script>
import BannerSection from "./BannerSection.vue"
export default {
    name: 'TheMain',
    components: {
        BannerSection
    },
    props: {
        bannerAdvs: Array,
        bannerTeam: Array
    }
}
</script>

<style>

</style>