<template>
  <button type="button" class="btn btn-warning fw-bold">{{ buttonText }}</button>
</template>

<script>
export default {
    name: 'BaseButton',
    props: {
        buttonText: String,
    },
}
</script>

<style scoped>
    .btn{
        border-radius: 0;
    }

    .btn-warning{
        background-color: #333333;
        border-color: #333333;
        color: white;
    }
</style>