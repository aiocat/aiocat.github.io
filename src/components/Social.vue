<!--
 Copyright (c) 2022 aiocat
 
 This software is released under the MIT License.
 https://opensource.org/licenses/MIT
-->

<script setup lang="ts">
</script>

<template>
    <div id="social">
        <h1>Social</h1>
        <span>
            <div class="account deviantart">
                <img src="/deviantart.svg" alt="deviantArt">
                <a target="_blank" href="https://www.deviantart.com/aiocat">aiocat</a>
            </div>
            <div class="account discord">
                <img src="/discord.svg" alt="discord">
                <a target="_blank" href="https://discord.com/users/872202276297637928">sec</a>
            </div>
            <div class="account github">
                <img src="/github.svg" alt="github">
                <a target="_blank" href="https://github.com/aiocat">0x707</a>
            </div>
            <div class="account osu">
                <img src="/osu.svg" alt="osu">
                <a target="_blank" href="https://osu.ppy.sh/users/28439842">111sec</a>
            </div>
            <div class="account twitter">
                <img src="/twitter.svg" alt="twitter">
                <a target="_blank" href="https://twitter.com/aiocat420">aiocat420</a>
            </div>
        </span>
    </div>
</template>

<style scoped>
#social {
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

span {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
}

.account {
    background: #1e1e2e;
    margin: 10px;
    border-radius: 10px;
    padding: 5px;

    display: flex;
    align-items: center;
    transition: 250ms;
}

.account img {
    width: 32px;
    height: 32px;
    margin: 5px;
    filter: invert(84%) sepia(5%) saturate(914%) hue-rotate(317deg) brightness(111%) contrast(92%);
}

.account a {
    color: #cdd6f4;
    font-size: 24px;
    font-weight: 700;
    text-decoration: none;
    margin: 5px;
}

.account:hover {
    background: #181825;
}
</style>
