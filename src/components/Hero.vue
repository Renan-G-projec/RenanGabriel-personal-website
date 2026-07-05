<!-- Ad Maiorem Dei Gloriam! -->

<script setup>
    import { onMounted, ref } from 'vue';

    const defaultString = "Just a beginner JS and C/C++ student";
    const showedString = ref("");
    const delayBetween = 70;
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
    <h1>{{ showedString }}</h1>
</template>