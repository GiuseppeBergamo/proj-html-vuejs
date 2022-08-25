<template>
  <div id="form" class="mb-2">
    <div class="container px-5 h-100">
        <div class="row row-cols-4 h-100 justify-content-center align-items-center">
            <div class="col">
                <input type="text" :placeholder="placeholder">
            </div>
            <div class="col">
                <input type="date">
            </div>
            <div class="col">
                <input type="time">
            </div>
            <div class="col">
                <BaseButton :buttonText="buttonText"></BaseButton>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
import BaseButton from './BaseButton.vue';
export default {
    name: "FormSection",
    data() {
        return {
            buttonText: "BOOK A TABLE"
        };
    },
    components: { BaseButton },
    props: {
        placeholder: String
    }
}
</script>

<style scoped>
#form {
    height: 200px;
    background-image: url('../assets/img/h3-background-img-3.jpg');
    background-repeat: no-repeat;
    background-size: cover;
}

input{
    padding: 10px 15px;
    border-radius: 0%;
    border: 2px solid black;
}
</style>