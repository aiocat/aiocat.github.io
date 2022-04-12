<!--
 Copyright (c) 2022 aiocat
 
 This software is released under the MIT License.
 https://opensource.org/licenses/MIT
-->



<script setup lang="ts">
import Navbar from './components/Navbar.vue'
import About from './components/About.vue'
import Projects from './components/Projects.vue'
</script>

<template>
  <Navbar />
  <About />
  <Projects />
</template>

<style>
html,
body,
#app {
  margin: 0 auto;
  font-family: 'Nunito', sans-serif;
  background-color: #030303;
  padding: 5px;
  box-sizing: border-box;
}
</style>
