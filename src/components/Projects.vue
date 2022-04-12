<!--
 Copyright (c) 2022 aiocat
 
 This software is released under the MIT License.
 https://opensource.org/licenses/MIT
-->

<script setup lang="ts">
import ProjectCard from './ProjectCard.vue'
</script>

<template>
    <div id="projects">
        <h1>Projects</h1>
        <div class="list">
            <ProjectCard title="This" desc="This website!" repo="aiocat.github.io" prog="Vue" />
            <ProjectCard title="Virna" desc="A programming language designed to be stack-based and concatenative with reverse polish notation" repo="virna" prog="Cpp" />
            <ProjectCard title="Request" desc="Minimal HTTP client with web interface" repo="request" prog="TS" />
            <ProjectCard title="GcWin" desc="Global command manager for Windows" repo="gcwin" prog="Cpp" />
            <ProjectCard title="Webcord" desc="Chrome extension to use themes in discord web" repo="webcord" prog="JS" />
            <ProjectCard title="Args" desc="Anonymous argument sharing and advocacy platform" repo="args" prog="Go" />
            <ProjectCard title="Axis" desc="CLI tool for find text from files" repo="axis" prog="Rust" />
            <ProjectCard title="Doomake" desc="Makefile clone less than 50 line" repo="doomak" prog="C" />
            <ProjectCard title="Solute" desc="Github-like avatar creator library" repo="solute" prog="Rust" />
            <ProjectCard title="Pixasso" desc="Reddit place like website written in one day" repo="pixasso" prog="Go" />
            <ProjectCard title="JDW" desc="Dynamic windows library for vanilla-js" repo="jdw" prog="JS" />
        </div>
    </div>
</template>

<style scoped>
div {
    width: 100%;
    padding: 10px;
    box-sizing: border-box;
    text-align: center;

    margin: 0px auto;
}

h1 {
    color: #fff;
    font-size: 48px;
    font-weight: 800;
}

.list {
    display: flex;
    flex: 1 1 25%;
    flex-direction: row;
    flex-wrap: wrap;
}
</style>
