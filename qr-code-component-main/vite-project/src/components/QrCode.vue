<script setup lang="ts">
import img from "../assets/image-qr-code.png";
</script>

<template>
    <div class="container">
        <div class="card">
            <img :src="img" alt="">
            <h3>Improve your front-end skills by building projects</h3>
            <p>Scan the QR code to visit Frontend Mentor and take your coding skills to the next level</p>
        </div>
        <div class="attribution">
            Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>.
            Coded by <a href="https://github.com/victor-web-dev">Victor E</a>.
        </div>
    </div>
</template>

<style scoped>
.container {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    height: 100vh;
    width: 100vw;
    background-color: var(--Lightgray);
}

.card {
    background-color: var(--White);
    text-align: center;
    border-radius: 20px;
    width: 300px;
    height: 475px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.card img {
    width: 90%;
    border-radius: 10px;
}

.card h3 {
    font-weight: 700;
    font-size: 1.5rem;
    color: var(--Dark-blue);
}

.card p {
    font-weight: 400;
    text-align: center;
    line-break: strict;
    letter-spacing: 0.5px;
    font-weight: 400;
    color: var(--Grayish-blue);
}

.card h3,
.card p {
    padding: 15px;
}

.attribution {
    font-size: 11px;
    text-align: center;
    margin-top: 15px;
}

.attribution a {
    color: hsl(228, 45%, 44%);
}
</style>