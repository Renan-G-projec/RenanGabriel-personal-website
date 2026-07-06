<!-- Ad Maiorem Dei Gloriam! -->

<template>
    <div class="about">
        <div class="content">
            <h2>About Me</h2>
            <p>
                I am a 15 year old programmer from Brazil. 
                I live in the north of <em>Santa Catarina</em> 
                and i love code since i was 10.
                My goal is to study abroad , work as a
                software engineer and help the world to become
                a better place. I'm also passionated about 
                the universe, the galaxies and mechanic enginering.
                I love understanding how things work by inside, and 
                i'm a Roman Catholic.
            </p>
        </div>
        
        <div class="img-container">
            <img src="../assets/img/catCode.jpg" alt="A cat with a qr code">
        </div>
    </div>
</template>

<style scoped>
    .about {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        margin-top: 4rem;
    }

    .content {
        width: clamp(20rem, 60vw, 100vw);
    }
</style>