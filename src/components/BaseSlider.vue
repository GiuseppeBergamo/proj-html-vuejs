<template>
  <div id="slider">
    <div class="d-flex align-items-center justify-content-center">
        <button type="button" id="prev" class="btn btn-light" @click="goToPrev">PREV</button>

        <div id="content">
            <div v-if="items[0].url">
                <img v-for="(item, index) in items" :key="index" :src="item.url" alt="urban-tastes" class="img-fluid" :class="{'active' : currentIndex === index}">
            </div>
            <div v-else class="container p-4 overflow-hidden">
                <div v-for="(item, index) in items" :key="index" id="quotes" class="text-center p-5" :class="{'active' : currentIndex === index}">
                    
                        
                    <h1 class="icon">"</h1>
                    <p class="fw-bold h4">"{{ item.text }}"</p>
                    <p id="subtitle" class="fw-bold">{{ item.author }}</p>
                        
                    
                </div>
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
    min-height: 300px;
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

#content .container{
    height: 300px;
}

#quotes{
    display: none;
}

#content #quotes.active{
    display: block;
}

#subtitle{
    font-size: 12px;
    color: #333333;
}

.icon{
    display: inline-block;
    font-size: 80px;
    color: #b7903c;
}

.btn{
    color: #333333;
    border-top-left-radius: 110px;
    border-top-right-radius: 110px;

}

.btn:hover {
    color: #333333;;
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