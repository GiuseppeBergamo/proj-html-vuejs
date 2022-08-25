<template>
    <div class="col">
        <img :src="card.url" :alt="card.id" class="img-fluid">
    </div>
</template>

<script>
export default {
    name: 'BannerCard',
    props: {
        card: Object,
    }
}
</script>

<style>

</style>