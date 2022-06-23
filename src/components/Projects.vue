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
        title="This"
        desc="This website!"
        repo="aiocat.github.io"
        prog="Vue"
      />
      <ProjectCard
        title="Doomake"
        desc="Makefile clone less than 50 line"
        repo="doomake"
        prog="C"
      />
      <ProjectCard
        title="Str"
        desc="Fast and flexible C library for string manupilation"
        repo="str"
        prog="C"
      />
      <ProjectCard
        title="GcWin"
        desc="Global command manager for Windows"
        repo="gcwin"
        prog="C++"
      />
      <ProjectCard
        title="Pixasso"
        desc="Anarchic pixel art website"
        repo="pixasso"
        prog="Go"
      />
      <ProjectCard
        title="Webcord"
        desc="Chromium extension to use themes in Discord Web"
        repo="webcord"
        prog="JS"
      />
      <ProjectCard
        title="Ctx"
        desc="Simple terminal-based text editor"
        repo="ctx"
        prog="Rust"
      />
      <ProjectCard
        title="Jel"
        desc="Flexible and memory-safe interpreted programming language"
        repo="cjel"
        prog="Rust"
      />
      <ProjectCard
        title="RipAC"
        desc="Cross-platform auto-clicker with GUI"
        repo="ripac"
        prog="Rust"
      />
      <ProjectCard
        title="RipGVC"
        desc="GitHub profile visitor counter"
        repo="ripgvc"
        prog="Rust"
      />
      <ProjectCard
        title="Taixoxo"
        desc="osu!taiko bot for Windows"
        repo="taixoxo"
        prog="Rust"
      />
      <ProjectCard
        title="DLL Crab"
        desc="Rusty DLL Injector with GUI"
        repo="dll-crab"
        prog="Rust"
      />
      <ProjectCard
        title="Request"
        desc="Minimal HTTP client with Vue3 front-end"
        repo="request"
        prog="Rust"
      />
      <ProjectCard
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
  color: #cdd6f4;
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
