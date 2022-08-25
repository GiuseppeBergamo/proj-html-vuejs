<template>
  <section id="pizzas" class="container py-5 mb-2">
    <div class="row mb-3">
        <div class="col-12 text-center">
            <p class="fs-small text-darkgrey fw-bold">CHOOSE YOUR FLAVOR</p>
            <h3 class="fw-bold mb-3">THE BEST PIZZA MENU IN TOWN</h3>
            <p class="text-grey">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nobis ullam, blanditiis in sed reiciendis dolorum accusantium aliquam quas officiis beatae magni placeat quaerat.</p>
        </div>
    </div>
    <div class="row row-cols-6">
        <div v-for="item in items" :key="item.id" class="col text-center">
            <img :src="item.url" :alt="item.name">
            <p class="fw-bold text-gold mb-1">{{ item.name }}</p>
            <p class="fw-bold">{{ item.price }}</p>
        </div>
    </div>
  </section>
</template>

<script>
export default {
    name: 'PizzasSection',
    props: {
        items: Array
    }
}
</script>

<style scoped>
#pizzas{
    min-height: 500px;
}

.text-grey{
  color: #b2b2b2;
}

.text-darkgrey{
    color: #333333;
}

.fs-small{
  font-size: 12px;
}

.text-gold{
    color: #b7903c;
}

img{
    height: 150px;
    margin-bottom: 10px;
    cursor: pointer;
    transition: all 0.5s ease;
}

img:hover{
    transform: scale(1.3);
    margin-bottom: 20px;
}
</style>