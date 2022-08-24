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
        background-color: #d2401e;
        border-color: #d2401e;
        color: white;
    }
</style>