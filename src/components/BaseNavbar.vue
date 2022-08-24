<template>
  <div id="navbar" class="container">
    <div class="row p-4 h-100 align-items-center">
        <div class="col-2">
            <BaseButton :buttonText="buttonText"></BaseButton>
        </div>
        <div class="col-8">
            <ul class="d-flex justify-content-around align-items-center px-5">
                <li class="me-4 d-flex align-items-center"><img src="../assets/svg/svg-0.svg" alt="home" class="invert me-1"><a href="#" class="fs-small">HOME</a></li>
                <li class="me-3 ms-4"><a href="#" class="fs-small">PAGES</a></li>
                <li class="me-3"><a href="#" class="fs-small">MENU</a></li>
                <li class="d-flex justify-content-center"><img src="../assets/img/h5-logo-divided-header-dark.png" alt="logo" class="img-fluid w-50" id="logo"></li>
                <li class="me-3"><a href="#" class="fs-small">EVENT</a></li>
                <li class="me-3"><a href="#" class="fs-small">BLOG</a></li>
                <li class="me-3"><a href="#" class="fs-small">LANDING</a></li>
            </ul>
        </div>
        <div class="col-2">
            <ul class="d-flex">
                <li class="me-3 d-flex align-items-center"><img src="../assets/svg/svg-1.svg" alt="cart" class="invert me-1"><a href="#" class="fs-small">CART</a></li>
                <li><a href="#" class="fs-small">SEARCH</a></li>
            </ul>
        </div>
    </div>
  </div>
</template>

<script>
import BaseButton from './BaseButton.vue';
export default {
    name: "BaseNavbar",
    component: {
        BaseButton,
    },
    data(){
        return{
            buttonText: 'OrderOnline'
        }
    },
    components: { BaseButton },
}
</script>

<style scoped>
#navbar{
    height: 100px;
}

a:hover{
    color: #d2401e;
}

#logo{
    
    filter: invert(100%) sepia(100%) saturate(0%) hue-rotate(31deg) brightness(102%) contrast(102%);
}

.invert{
    filter: invert(100%)
}

.fs-small{
    font-size: 14px;
}
</style>