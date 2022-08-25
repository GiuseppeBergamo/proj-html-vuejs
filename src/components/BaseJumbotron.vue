<template>
  <section id="jumbotron" class="p-5 mb-2">
    <div class="d-flex justify-content-start align-items-center p-2">
        <div class="w-25 p-2">
            <h1 class="fw-bold text-white text-start">GO AHEAD AND BUILD YOUR OWN PIZZA</h1>
            <h1 class="fw-bold text-white text-start">WE WON'T JUDGE!</h1>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'BaseJumbotron',
}
</script>

<style scoped>
#jumbotron{
    height: 400px;
    background-image: url('../assets/img/h3-background-img.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
}
</style>