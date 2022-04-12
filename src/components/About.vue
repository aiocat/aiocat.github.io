<!--
 Copyright (c) 2022 aiocat
 
 This software is released under the MIT License.
 https://opensource.org/licenses/MIT
-->

<script setup lang="ts">
const imageUrl: string = new URL("../assets/pfp.png", import.meta.url).href
</script>

<template>
    <div id="about">
        <span class="profile">
            <h1>Aiocat</h1>
            <h2>(0x707)</h2>
            <p>I'm a software engineer with over 3+ years of experience from Turkey. I don't have a tech stack, I 🤗 all
                of them <span>except php</span>. I mostly code to solve my problems.</p>
        </span>
        <span class="photo">
            <img :src="imageUrl" alt="pfp">
            <p>(I love GitHub's default avatar)</p>
        </span>
    </div>
</template>

<style scoped>
div {
    width: 100%;
    padding: 50px;
    box-sizing: border-box;

    display: flex;
    align-items: center;
    justify-content: space-around;

    margin: 0px auto;
}

.profile,
.photo {
    margin: 50px;
}

.profile h1 {
    color: #fff;
    font-size: 36px;
    font-weight: 800;
    margin: 0px;
}

.profile h2 {
    color: #bbb;
    font-size: 16px;
    font-weight: 600;
    margin: 0px;
}

.profile p {
    color: #ddd;
    font-size: 24px;
    font-weight: 700;

    margin: 0px;
    margin-top: 20px;
}

.profile p span {
    color: rgb(255, 70, 70);
    font-size: 14px;
    font-weight: 600;
}

.photo img {
    display: block;
    width: 128px;
    image-rendering: pixelated;
    border-radius: 10px;
    margin: 0 auto;
    box-shadow: rgba(255, 255, 255, 0.432) 0px 3px 8px;
}

.photo p {
    display: block;

    color: #bbb;
    font-size: 14px;
    font-weight: 600;
    text-align: center;
}

@media only screen and (max-width: 800px) {
    div {
        flex-wrap: wrap-reverse;
    }
}
</style>
