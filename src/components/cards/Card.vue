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