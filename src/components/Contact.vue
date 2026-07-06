<!-- Ad Maiorem Dei Gloriam! -->

<template>
    <div class="contact">
        <div class="content">
            <h2>Contact Me!</h2>
            <div class="icons">
                <div class="icon-pack">
                    <div class="icon"><a href="https://github.com/Renan-G-projec"><img src="/src/assets/img/githubicon.png" alt="Github Icon"></a></div>
                    <p>Github: Renan-G-projec</p>
                </div>
                <div class="icon-pack">
                    <div class="icon"><a href="mailto:renanfartes@gmail.com"><img src="/src/assets/img/gmailicon.png" alt="Gmail Icon"></a></div>
                    <p>E-mail: renanfartes@gmail.com</p>
                </div>
            </div>
        </div>
        
        <div class="img-container">
            <img src="/src/assets/img/contact.jpg" alt="A telephone image">
        </div>
    </div>
</template>

<style scoped>
    h3 {
        margin-bottom: 2rem;
    }
    .contact {
        display: flex;
        justify-content: space-between;
        margin: 4rem 7rem;
        gap: 3rem;
    }

    .img-container {
        width: 20rem;
    }

    .icon-pack {
        display: flex;
    }

    .icon {
        background-color: rgb(64, 64, 124);
        padding: 1rem;
        border-radius: 50%;
        margin-right: 1rem;

        width: 3rem;
        height: 3rem;
        text-align: center;
    }

    .icons {
        display: flex;
        flex-direction: column;
        gap: 1rem;
    }

    a img {
        width: 2.7rem;
    }
    
    p {
        display: flex;
        align-items: center;
    }
</style>