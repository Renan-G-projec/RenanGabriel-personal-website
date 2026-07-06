<!-- Ad Maiorem Dei Gloriam! -->

<script setup>
    defineProps({
        title: String,
        img: String
    })
</script>

<template>
    <div class="card">
        <div class="img-container">
            <img :src="img" :alt="title">
        </div>
        <div class="content">
            <h3>{{  title }}</h3>
            <slot></slot>
        </div>
    </div>
</template>

<style scoped>
    .card {
        width: clamp(20rem, 25vw, 50rem);
        height: 40vh;
        overflow: hidden;

        border-radius: 1rem;
    }

    .img-container {
        height: 30%;
        overflow: hidden;
    }

    .content {
        margin: 0.7rem;
    }

    h3 {
        font-size: 1.4rem;
    }

</style>