<template>
  <div id="split-footer" class="w-100 d-flex">
    <div class="w-50 p-5 h-100 d-flex justify-content-center align-items-center">
        <div class="w-50">
            <ul>
                <li><h4 class="fw-bold text-gold">{{ title }}</h4></li>
                <li v-for="item in items" :key="item.id" class="mb-2">
                    <p class="text-gold fw-bold">{{ item.day }}</p>
                    <p class="text-grey" :class="{ 'text-orange' : item.text }">{{ item.text || item.hour }}</p>
                </li>
                <li>
                    <p class="text-grey">FOLLOW US: </p>
                </li>
            </ul>
        </div>
        <div class="w-50 h-100">
            <h3 class="text-white text-start">
                THE DON PEPPE CREW FIRST AND FOREMOST VALUES AN AUTHENTIC, WELL BAKED SLICE OF PIZZA.
            </h3>
        </div>
    </div>
    <div class="w-50" id="image">

    </div>
  </div>
</template>

<script>
export default {
    name: 'SplitSectionThird',
    props: {
        items: Array,
        title: String
    }
}
</script>

<style scoped>
#split-footer{
    min-height: 600px;
    background-color: #1a1a1a;
}

.text-gold{
    color: #b7903c;
}

.text-orange{
    color: #ab4027;
}

.text-grey{
  color: #b2b2b2;
}

#image{
    background-image: url('../assets/img/footer-img-1.jpg');
    background-repeat: no-repeat;
    background-size: cover;
}
</style>