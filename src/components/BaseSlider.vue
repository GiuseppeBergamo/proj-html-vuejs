<template>
  <div id="slider">
    <div class="d-flex align-items-center justify-content-center">
        <button type="button" id="prev" class="btn btn-light" @click="goToPrev">PREV</button>

        <div id="content">
            <div v-if="items[0].url">
                <img v-for="(item, index) in items" :key="index" :src="item.url" alt="urban-tastes" class="img-fluid" :class="{'active' : currentIndex === index}">
            </div>
            <div v-else>
                
            </div>
        </div>

        <button type="button" id="next" class="btn btn-light" @click="goToNext">NEXT</button>
    </div>
  </div>
</template>

<script>
export default {
    name: "BaseSlider",
    data() {
        return {
            currentIndex: 0,
        };
    },
    props: {
        items: Array
    },
    methods: {
        goToPrev() {
            this.currentIndex--;
            if (this.currentIndex < 0) {
                this.currentIndex = 2;
            }
        },
        goToNext() {
            this.currentIndex++;
            if (this.currentIndex == this.items.length) {
                this.currentIndex = 0;
            }
        }
    },
}
</script>

<style scoped>
#slider{
    width: 100%;
    height: 500px;
    overflow-x: hidden;
    position: relative;
}

img{
    height: 450px;
    display: none;
}

#content img.active{
    display: block;
}

.btn{
    color: #d2401e;
    border-top-left-radius: 110px;
    border-top-right-radius: 110px;

}

.btn:hover {
    color: #d2401e;;
}

#prev {
    transform: rotate(90deg);
    position: absolute;
    left: -20px;
}

#next {
    transform: rotate(-0.25turn);
    position: absolute;
    right: -20px;
}
</style>