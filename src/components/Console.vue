<!--
 Copyright (c) 2022 aiocat
 
 This software is released under the MIT License.
 https://opensource.org/licenses/MIT
-->

<script setup lang="ts">
import { ref } from "vue";

const stdin = ref<string>("");
const stdout = ref<string>("");

function executeShell(): void {
    const splitted: Array<string> = stdin.value.split(" ");

    switch (splitted[0]) {
        case "clear":
        case "cls":
            stdout.value = "";
            break;
        case "projects":
            window.location.href = "#projects";
            break;
        case "about":
            window.location.href = "#about";
            break;
        case "social":
            window.location.href = "#social";
            break;
        case "echo":
            if (splitted.length < 2) {
                stdout.value = "error: need one more parameter to run echo";
                break;
            }

            stdout.value = splitted.filter((i: string): boolean => i != "echo").join(" ")
            break;
        case "hack":
            window.location.href = "https://github.com/aiocat/aiocat.github.io";
            stdout.value = "😎😎😎 WebS1t3 iz H4cK3d by 1337kidz 😎😎😎";
            break;
        case "source":
            window.location.href = "https://github.com/aiocat/aiocat.github.io";
            break;
        case "root":
            window.location.href = "https://github.com/aiocat";
            break;
        case "help":
            stdout.value = "dear 73.245.74.36, please check the Console.vue file in the source code.";
            break;
        case "whoami":
            stdout.value = "dear 73.245.74.36, i don't know you (yet)";
            break;
    }

    stdin.value = "";
}
</script>

<template>
    <div id="console">
        <h1>Console</h1>
        <div id="shell">root: <input placeholder="help" spellcheck="false" type="text" id="stdin" v-model="stdin" @keyup.enter="executeShell">
        <div id="stdout">{{ stdout }}</div>
        </div>
    </div>
</template>

<style scoped>
#console {
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

#shell {
    width: 50%;
    height: 50vh;
    margin: 0 auto;

    background: #1e1e2e;
    color: #f5e0dc;
    border-radius: 10px;

    padding: 10px;

    font-family: 'Roboto Mono', monospace;
    text-align: left;
    font-weight: 600;
    font-size: 18px;
    overflow: auto;
}

#stdout {
    color: #f5e0dc;
    font-size: 14px;
    font-weight: 500;
    padding: 10px;
    box-sizing: border-box;
}

#shell #stdin {
    width: 70%;
    font-family: 'Roboto Mono', monospace;

    border: none;
    outline: none;

    background: transparent;
    color: #f5e0dc;

    padding: 0px;
    margin: 0px;
    font-weight: 500;
    font-size: 18px;
}

::placeholder {
  color: #45475a;
  opacity: 1;
}


@media only screen and (max-width: 800px) {
    #shell {
        width: 80%;
    }
}
</style>
