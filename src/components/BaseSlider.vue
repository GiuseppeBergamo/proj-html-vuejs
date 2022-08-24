<template>
  <div id="slider">
    <div class="d-flex align-items-center justify-content-center">
        <button type="button" id="prev" class="btn btn-light" @click="goToPrev">PREV</button>

        <div id="content">
            <img v-for="(image, index) in urbanTastesImages" :key="index" :src="image.url" alt="urban-tastes" class="img-fluid" :class="{'active' : currentIndex === index}">
        </div>

        <button type="button" id="next" class="btn btn-light" @click="goToNext">NEXT</button>
    </div>
  </div>
</template>

<script>
export default {
    name: 'BaseSlider',
    data(){
        return {
            currentIndex: 0,
            urbanTastesImages: [
                {
                    url: require('../assets/img/h3-rev-img-6.png')
                },
                {
                    url: require('../assets/img/h3-rev-img-4.png')
                },
                {
                    url: require('../assets/img/h3-rev-img-2.png')
                }
            ]
        }
    },
    methods: {
        goToPrev(){
            this.currentIndex--;
            if (this.currentIndex < 0) {
                this.currentIndex = 2;
            }
        },
        goToNext(){
            this.currentIndex++;
            if (this.currentIndex == this.urbanTastesImages.length) {
                this.currentIndex = 0
            }
        }
    }
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