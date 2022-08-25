<template>
    <section id="split-section" class="mb-2 d-flex w-100">
        <div id="content" class="w-50 p-5 d-flex justify-content-center align-items-center">
            <ul class="text-start p-2">
                <li id="title">
                    <ul>
                        <li><p class="fs-small text-orange fw-bold">{{ smallTitle }}</p></li>
                        <li><h1 class="h2 fw-bold text-white">{{ title }}</h1></li>
                    </ul>
                </li>
                <li id="item" v-for="item in items" :key="item.id" class="my-4">
                    <div class="row">
                        <div class="col-2">
                            <h2 class="fw-bold text-orange">{{ item.day }}</h2>
                            <h3 class="fw-bold text-white">{{ item.month }}</h3>
                        </div>
                        <div class="col-10">
                            <h3 class="fw-bold text-white">{{ item.title }}</h3>
                            <p class="fs-small text-orange">{{ item.location }}</p>
                        </div>
                    </div>
                </li>
            </ul>
        </div>
        <div id="image" class="w-50">
            
        </div>
    </section>
</template>

<script>
export default {
    name: 'SplitSectionSecond',
    props: {
        items: Array,
        title: String,
        smallTitle: String
    }
}
</script>

<style scoped>
#split-section {
  min-height: 600px;
  background-color: #1a1a1a;
}

#image{
    background-image: url('../assets/img/h3-img-5a.jpg');
    background-size: cover;
    background-repeat: no-repeat;
}

#item{
    border-bottom: #b7903c 2px dotted;
}

.text-orange{
    color: #ab4027;
}

.text-gold{
    color: #b7903c;
}

.fs-small{
  font-size: 12px;
}
</style>