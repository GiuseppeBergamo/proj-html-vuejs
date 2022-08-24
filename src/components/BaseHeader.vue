<template>
    <header>
        <BaseNavbar></BaseNavbar>
        <BaseSlider></BaseSlider>
    </header>
</template>

<script>
import BaseNavbar from './BaseNavbar.vue'
import BaseSlider from './BaseSlider.vue'
export default {
    name: 'BaseHeader',
    components: {
        BaseNavbar,
        BaseSlider
    },
    
    
}   
</script>

<style scoped>
header{
    min-height: 600px;
    background-color: #1B1B1B;
    background-image: url(../assets/img/h3-rev-img-5.png);
    background-repeat: no-repeat;
    background-position: center;
    background-size: 50%;

}
</style>