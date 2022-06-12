<!--
 Copyright (c) 2022 aiocat
 
 This software is released under the MIT License.
 https://opensource.org/licenses/MIT
-->

<script setup lang="ts">
import ProjectCard from "./ProjectCard.vue";
</script>

<template>
  <div id="projects">
    <h1>Projects</h1>
    <div class="list">
      <ProjectCard
        mark="gold"
        title="This"
        desc="This website!"
        repo="aiocat.github.io"
        prog="Vue"
      />

      <ProjectCard
        mark=""
        title="Doomake"
        desc="Makefile clone less than 50 line"
        repo="doomake"
        prog="C"
      />
      <ProjectCard
        mark=""
        title="Str"
        desc="Fast and flexible C library for string manupilation"
        repo="str"
        prog="C"
      />
      <ProjectCard
        mark=""
        title="GcWin"
        desc="Global command manager for Windows"
        repo="gcwin"
        prog="Cpp"
      />
      <ProjectCard
        mark=""
        title="Virna"
        desc="A programming language designed to be stack-based and concatenative with reverse polish notation"
        repo="virna"
        prog="Cpp"
      />
      <ProjectCard
        mark=""
        title="Args"
        desc="Anonymous argument sharing and advocacy platform"
        repo="args"
        prog="Go"
      />
      <ProjectCard
        mark=""
        title="Pixasso"
        desc="Reddit place like website written in one day"
        repo="pixasso"
        prog="Go"
      />
      <ProjectCard
        mark=""
        title="Webcord"
        desc="Chrome extension to use themes in discord web"
        repo="webcord"
        prog="JS"
      />
      <ProjectCard
        mark=""
        title="JDW"
        desc="Dynamic windows library for vanilla-js"
        repo="jdw"
        prog="JS"
      />
      <ProjectCard
        mark="gold"
        title="RipAC"
        desc="Cross-platform auto-clicker written in Rust"
        repo="ripac"
        prog="Rust"
      />
      <ProjectCard
        mark="gold"
        title="RipGVC"
        desc="GitHub profile visitor counter"
        repo="ripgvc"
        prog="Rust"
      />
      <ProjectCard
        mark=""
        title="Jel"
        desc="Flexible, memory-safe, easy-to-use, interpreted programming language"
        repo="jel"
        prog="Rust"
      />
      <ProjectCard
        mark="gold"
        title="Taixoxo"
        desc="osu!taiko bot for Windows"
        repo="taixoxo"
        prog="Rust"
      />
      <ProjectCard
        mark=""
        title="Axis"
        desc="CLI tool for find text from files"
        repo="axis"
        prog="Rust"
      />
      <ProjectCard
        mark="gold"
        title="DLL Crab"
        desc="Rusty DLL Injector with GUI"
        repo="dll-crab"
        prog="Rust"
      />
      <ProjectCard
        mark="gold"
        title="Request"
        desc="Minimal HTTP client with Vue3 front-end"
        repo="request"
        prog="Rust"
      />
      <ProjectCard
        mark=""
        title="Solute"
        desc="Github-like avatar creator library"
        repo="solute"
        prog="Rust"
      />
      <ProjectCard
        mark=""
        title="Totify"
        desc="Lightweight notification creator for browser"
        repo="totift"
        prog="TS"
      />
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
