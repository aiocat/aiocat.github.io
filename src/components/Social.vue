<!--
 Copyright (c) 2022 aiocat
 
 This software is released under the MIT License.
 https://opensource.org/licenses/MIT
-->

<script setup lang="ts">
const deviantArtUrl: string = new URL("../../public/deviantart.svg", import.meta.url).href
const discordUrl: string = new URL("../../public/discord.svg", import.meta.url).href
const githubUrl: string = new URL("../../public/github.svg", import.meta.url).href
const osuUrl: string = new URL("../../public/osu.svg", import.meta.url).href
const twitterUrl: string = new URL("../../public/twitter.svg", import.meta.url).href
</script>

<template>
    <div id="social">
        <h1>Social</h1>
        <span>
            <div class="account deviantart">
                <img :src="deviantArtUrl" alt="deviantArt">
                <a href="https://www.deviantart.com/aiocat">Aiocat</a>
            </div>
            <div class="account discord">
                <img :src="discordUrl" alt="discord">
                <a href="https://discord.com/users/872202276297637928">sec</a>
            </div>
            <div class="account github">
                <img :src="githubUrl" alt="github">
                <a href="https://github.com/aiocat">0x707</a>
            </div>
            <div class="account osu">
                <img :src="osuUrl" alt="osu">
                <a href="https://osu.ppy.sh/users/28439842">111sec</a>
            </div>
            <div class="account twitter">
                <img :src="twitterUrl" alt="twitter">
                <a href="https://twitter.com/aiocat420">aiocat420</a>
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
    color: #fff;
    font-size: 48px;
    font-weight: 800;
}

span {
    display: flex;
    align-items: center;
    justify-content: center;
}

.account {
    background: #0a0a0a;
    border: 4px solid #111;
    margin: 10px;
    border-radius: 10px;
    padding: 0px 5px 0px 5px;
    box-shadow: rgb(0, 0, 0) 0px 3px 8px;

    display: flex;
    align-items: center;
}

.account img {
    width: 32px;
    height: 32px;
    margin: 5px;
    filter: invert(99%) sepia(3%) saturate(150%) hue-rotate(244deg) brightness(116%) contrast(100%);
}
.account a {
    color: #fff;
    font-size: 24px;
    font-weight: 700;
    text-decoration: none;
    margin: 5px;
}

.deviantart:hover > img, .deviantart:hover > a { 
    filter: invert(50%) sepia(99%) saturate(903%) hue-rotate(96deg) brightness(98%) contrast(96%);
}

.discord:hover > img, .discord:hover > a { 
    filter: invert(42%) sepia(89%) saturate(5009%) hue-rotate(228deg) brightness(107%) contrast(90%);
}

.osu:hover > img, .osu:hover > a { 
    filter: invert(57%) sepia(46%) saturate(1719%) hue-rotate(298deg) brightness(101%) contrast(101%);
}
.twitter:hover > img, .twitter:hover > a { 
    filter: invert(57%) sepia(28%) saturate(7158%) hue-rotate(178deg) brightness(102%) contrast(90%);
}
</style>
