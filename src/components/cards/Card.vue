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
            <p><slot></slot></p>
        </div>
    </div>
</template>

<style scoped>
    .card {
        width: clamp(20rem, 25vw, 50rem);
        height: 17rem;
        overflow: hidden;

        border-radius: 1rem;
    }

    h3 {
        text-align: left;
    }

    .img-container {
        height: 30%;
        overflow: hidden;

        cursor: pointer;
    }

    img {
        width: 100%;
        object-fit: cover;
        transition: transform 0.3s ease-in-out;
    }

    img:hover {
        transform: scale(1.1);
    }

    .content {
        padding: 0.9rem;
        height: 100%;
        color: black;
        background-color: white;
    }

    h3 {
        font-size: 1.4rem;
    }

    p {
        font-size: 1rem;
    }
</style>