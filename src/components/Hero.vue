<!-- Ad Maiorem Dei Gloriam! -->

<script setup>
    import { onMounted, ref } from 'vue';

    const defaultString = "Just a beginner JS and C/C++ student";
    const showedString = ref("");
    const delayBetween = 40;
    let charactersNumber = 0;
    
    function typewritterStep() {
        showedString.value += defaultString[charactersNumber];
        charactersNumber++;
    }

    onMounted(() => {
        const interval = setInterval(() => {
            if (charactersNumber < defaultString.length) {
                typewritterStep();
            } else {
                clearInterval(interval);
            }
        }, delayBetween)
    })
</script>

<template>
    <div class="hero">
        <div class="content">
            <h1>Renan Gabriel</h1>
            <h2>{{ showedString }}</h2>
        </div>

        <div class="pfp-container">
            <img src="../assets/profileImage.jpg" alt="My pfp">
        </div>

    </div>
</template>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Passero+One&display=swap');

    .hero {
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
    }

    h1, h2 {
        margin: 0;

        font-family: "Passero One", sans-serif;
        font-style: normal;
    }
    h1 {
        font-size: 7rem;
    }

    .pfp-container {
        overflow: hidden;

        border-radius: 50%;
    }

    img {
        height: 14rem;
        width: 14rem;

        object-fit: cover;

        transform: scale(1.1);
        transform-origin: 50% 50%;
    }
</style>