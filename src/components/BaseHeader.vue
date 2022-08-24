<template>
    <header>
        <BaseNavbar></BaseNavbar>
    </header>
</template>

<script>
import BaseNavbar from './BaseNavbar.vue'

export default {
    name: 'BaseHeader',
    components: {
        BaseNavbar,
    },
    
}   
</script>

<style scoped>
header{
    height: 600px;
    background-color: #1B1B1B;
   

}
</style>