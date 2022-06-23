<!--
 Copyright (c) 2022 aiocat
 
 This software is released under the MIT License.
 https://opensource.org/licenses/MIT
-->

<script setup lang="ts">
defineProps<{
    title: string,
    desc: string,
    repo: string,
    prog: string,
}>();
</script>

<template>
    <div class="card">
        <span>
            <a target="_blank" :href="`https://github.com/aiocat/${repo}`">{{ title }}</a>
            <span class="tag">
                <p>{{ prog }}</p>
                <div :class="['round', prog]"></div>
            </span>
        </span>
        <p>{{ desc }}</p>
    </div>
</template>

<style scoped>
.card {
    background: #1e1e2e;
    flex: 1 1 25%;
    margin: 10px;
    border-radius: 10px;
    text-align: left;
    padding: 10px;

    transition: 200ms;
}

.card:hover {
    background: #181825;
}

.tag {
    background: #313244;
    padding: 2px 6px 2px 6px;
    border-radius: 10px;
    transition: 200ms;
}
.round {
    display: inline-block;
    width: 18px;
    height: 18px;
    border-radius: 10px;
    margin: 0px;
    margin-left: 5px;
}

span {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin: 0px;
}

a {
    color: #cdd6f4;
    font-size: 24px;
    font-weight: 800;
    margin: 0px;
    text-decoration: none;

    transition: 200ms;
}

a::after {
    content: "(click)";
    font-size: 14px;
    font-weight: 700;
    margin-left: 5px;

    color: #bac2de;
}

p {
    color: #a6adc8;
    font-size: 18 px;
    font-weight: 700;
    margin: 0px;
}

.TS {
    background: #89b4fa;
}

.C\+\+ {
    background: #f38ba8;
}

.Go {
    background: #89dceb;
}

.C {
    background: #f5c2e7;
}

.JS {
    background: #f9e2af;
}

.Rust {
    background: #f5e0dc;
}

.Vue {
    background: #a6e3a1;
}
</style>
