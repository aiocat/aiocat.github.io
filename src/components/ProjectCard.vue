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

<script lang="ts">
export default {
    props: ["repo", "title", "desc", "prog"]
}
</script>

<template>
    <div class="card">
        <span>
            <a :href="`https://github.com/aiocat/${repo}`">{{ title }}</a>
            <span class="mark">
                <p>{{ prog }}</p>
                <div :class="['round', prog]"></div>
            </span>
        </span>
        <p>{{ desc }}</p>
    </div>
</template>

<style scoped>
.card {
    background: #0a0a0a;
    border: 4px solid #111;
    flex: 1 1 25%;
    margin: 10px;
    border-radius: 10px;
    text-align: left;
    padding: 10px;
    align-items: center;

    transition: 200ms;
}

.card:hover {
    background: #111;
}

.card:hover .mark {
    background: #222;
}

.mark {
    background: #1a1a1a;
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
    flex-wrap: wrap;
    margin: 0px;
}

a {
    color: #eee;
    font-size: 24px;
    font-weight: 800;
    margin: 0px;
    text-decoration: none;

    transition: 200ms;
}

a:hover {
    color: #fff;
}

p {
    color: #bbb;
    font-size: 18 px;
    font-weight: 700;
    margin: 0px;
}

.TS {
    background: #2b7489;
}

.Cpp {
    background: #f34b7d;
}

.Go {
    background: #00add8;
}

.C {
    background: #555555;
}

.JS {
    background: #f1e05a;
}

.Rust {
    background: #dea584;
}

.Vue {
    background: #41b883;
}
</style>
