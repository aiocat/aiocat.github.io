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
    mark: string
}>();
</script>

<script lang="ts">
export default {
    props: ["repo", "title", "desc", "prog", "mark"]
}
</script>

<template>
    <div :class="['card', mark]">
        <span>
            <a :href="`https://github.com/aiocat/${repo}`">{{ title }}</a>
            <span class="tag">
                <p>{{ prog }}</p>
                <div :class="['round', prog]"></div>
            </span>
        </span>
        <span>
            <p>{{ desc }}</p>
            <p v-if="mark === 'gold'" class="star">⭐️</p>
        </span>
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
    box-shadow: rgb(0, 0, 0) 0px 3px 8px;

    transition: 200ms;
}

.card:hover {
    background: #111;
}

.card:hover .tag {
    background: #222;
}

.star {
    display: inline-block;
    font-size: 20px;
    margin: 5px;
    animation: action 2s infinite ease-in-out alternate;
}

.gold {
    background: #1a1307;
    border: 4px solid rgb(255, 219, 60);
    box-shadow: rgba(255, 195, 31, 0.185) 0px 3px 8px;
}

.tag {
    background: #1a1a1a;
    padding: 2px 6px 2px 6px;
    border-radius: 10px;
    transition: 200ms;
}

.gold .tag {
    background: #2b210f;
}

.gold:hover {
    background: #20190c;
    border: 4px solid rgb(255, 229, 116);
}
.gold:hover .tag {
    background: rgb(63, 51, 31);
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

a::after {
    content: "(click)";
    font-size: 14px;
    font-weight: 700;
    margin-left: 5px;

    color: #888;
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

@keyframes action {
    0% { 
        transform: translateY(0px) rotate(20deg);
    }
    100% { 
        transform: translateY(5px) rotate(-20deg); 
    }
}
</style>
