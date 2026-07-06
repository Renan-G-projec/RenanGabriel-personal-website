<!-- Ad Maiorem Dei Gloriam! -->

<script setup>
    import Card from "./cards/Card.vue";

    const projects = [
        {
            title: "RenanG_OS",
            description: "A small browser-based Operational System Simulation!",
            link: "https://renang-os.netlify.app",
            github: "https://github.com/Renan-G-projec/RenanG_OS",
            img: ""
        }, 
        {
            title: "AsciiBird", 
            description: "A flappy bird game that runs entirely on the terminal!",
            link: "https://github.com/Renan-G-projec/AsciiBird/releases/tag/v1.0.0",
            github: "https://github.com/Renan-G-projec/AsciiBird",
            img: ""
        },
        {
            title: "ScopeCutter",
            description: "A tool, that helps developers prevent overengineering.",
            link: "https://scopecutter.netlify.app/",
            github: "https://github.com/Renan-G-projec/ScopeCutter",
            img: ""
        },
        {
            title: "WebLinuxTerminal",
            description: "A web-based unix-like terminal emulation to help new developers learn to work with it!",
            link: "https://github.com/Renan-G-projec/WebLinuxTerminal",
            github: "https://github.com/Renan-G-projec/WebLinuxTerminal",
            img: ""
        },
        {
            title: "Organizer",
            description: "CLI script that organizes files by their metadata in folders.",
            link: "https://github.com/Renan-G-projec/Organizer",
            github: "https://github.com/Renan-G-projec/Organizer",
            img: ""
        }
    ]
</script>

<template>
    <div class="projects">
        <h2>Projects</h2>
        <p>Here are some of my projects. They're simple, but made with love.</p>
    </div>

    <div class="projects-container">
        <div class="project" v-for="project in projects">
            <Card :title="project.title" :img="project.img">
                {{ project.description }} <br>
                Link: <a :href="project.link">{{ project.link }}</a> <br>
                Github: <a :href="project.github"> {{  project.github }}</a>
            </Card>
        </div>
    </div>
</template>


<style scoped>
    .projects-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;

        margin-top: 4rem;
    }
</style>