<!--
 Copyright (c) 2022 aiocat
 
 This software is released under the MIT License.
 https://opensource.org/licenses/MIT
-->



<script setup lang="ts">
import Navbar from "./components/Navbar.vue"
import About from "./components/About.vue"
import Projects from "./components/Projects.vue"
import Console from "./components/Console.vue"
import Social from "./components/Social.vue"
import Footer from "./components/Footer.vue"
</script>

<template>
  <Navbar />
  <About />
  <Projects />
  <Console />
  <Social />
  <Footer />
</template>

<style>
html,
body,
#app {
  margin: 0 auto;
  font-family: "Nunito", sans-serif;
  background-color: #11111b;
  padding: 5px;
  box-sizing: border-box;
  scroll-behavior: smooth;
}

::-webkit-scrollbar {
  width: 6px;
  height: 6px;
}

::-webkit-scrollbar-button {
  width: 0px;
  height: 0px;
}

::-webkit-scrollbar-thumb {
  background: #f5e0dc;
}

::-webkit-scrollbar-track {
  background: transparent;
}

::-webkit-scrollbar-track:hover {
  background: transparent;
}

::-webkit-scrollbar-track:active {
  background: transparent;
}

::-webkit-scrollbar-corner {
  background: transparent;
}
</style>
