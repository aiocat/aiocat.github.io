<!--
 Copyright (c) 2022 aiocat
 
 This software is released under the MIT License.
 https://opensource.org/licenses/MIT
-->

<template>
    <div id="about">
        <span class="profile">
            <h1>Aiocat</h1>
            <h2>(0x707)</h2>
            <p>I'm a software engineer with over 3+ years of experience from Turkey. I don't have a tech stack, I 🤗 all
                of them <span>except php</span>. Also i play Apeirophobia <span>roblox</span> so much.</p>
            <a href="mailto:aiocat@protonmail.com">Contact</a>
        </span>
        <span class="photo">
            <img src="/pfp.jpg" alt="pfp">
            <p>(nuclear bomb ☠️)</p>
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
    color: #cdd6f4;
    font-size: 36px;
    font-weight: 800;
    margin: 0px;
}

.profile h2 {
    color: #bac2de;
    font-size: 16px;
    font-weight: 600;
    margin: 0px;
}

.profile p {
    color: #a6adc8;
    font-size: 24px;
    font-weight: 700;

    margin: 0px;
    margin-top: 20px;
}

.profile p span {
    color: #eba0ac;
    font-size: 14px;
}

.photo img {
    display: block;
    width: 128px;
    image-rendering: pixelated;
    border-radius: 10px;
    margin: 0 auto;
    border: 4px solid #f5e0dc;
}

.photo p {
    display: block;

    color: #bac2de;
    font-size: 14px;
    font-weight: 600;
    text-align: center;
}

.profile a {
    background-color: #cdd6f4;
    padding: 5px 10px 5px 10px;
    border-radius: 10px;

    color: #11111b;
    font-size: 18px;
    font-weight: 600;
    
    text-decoration: none;

    display: inline-block;
    margin: 0px;
    margin-top: 10px;

    transition: 200ms;
}

.profile a:hover {
    background-color: #bac2de;
}

@media only screen and (max-width: 800px) {
    div {
        flex-wrap: wrap-reverse;
        padding: 10px;
        text-align: center;
    }
    .profile,
    .photo {
        margin: 20px;
    }
}
</style>
