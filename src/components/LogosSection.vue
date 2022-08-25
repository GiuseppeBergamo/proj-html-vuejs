<template>
  <section id="logos" class="mb-2 px-5">
    <div class="container h-100 d-flex justify-content-center align-items-center">
        <div class="row row-cols-5 px-5">
            <div v-for="item in items" :key="item.id" class="col">
                <img :src="item.url" :alt="item.id" class="img-fluid">
            </div>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'LogosSection',
    props: {
        items: Array,
    }
}
</script>

<style scoped>
#logos{
    height: 250px;
    background-color: #f7f7f2;
}
</style>