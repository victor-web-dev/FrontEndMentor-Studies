<script setup lang="ts"></script>

<template>
    <main class="container">
        <div class="card">
            <div class="image"></div>
            <div class="content">
                <h1>Perfume</h1>
                <h2>Gabrielle Essence Eau De Parfum</h2>
                <p>A floral, solar and voluptuous interpretation composed by Olivier Polge,
                    Perfumer-Creator for the House of CHANEL.</p>
                <div id="prices">
                    <span>$149.99</span>
                    <span>$169.99</span>
                </div>
                <button>
                    <img src="../assets/icon-cart.svg" class="btn-icon" alt="">
                    Add to Cart
                </button>
            </div>
        </div>
        <div class="attribution">
            Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>.
            Coded by <a href="https://github.com/victor-web-dev">Victor E</a>.
        </div>
    </main>
</template>

<style scoped>
.container {
    background-color: var(--cream);
    height: 100vh;
    width: 100vw;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.card {
    display: grid;
    grid-template-columns: 1fr 1fr;
    height: 500px;
    width: 650px;
    border-radius: 12px;
    background-color: var(--white);
}

.image {
    background-image: url("../assets/image-product-desktop.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    border-top-left-radius: 12px;
    border-bottom-left-radius: 12px;
}

.content {
    padding: 10%;
    text-align: left;
}

.content h1 {
    font-family: 'Montserrat', sans-serif;
    text-transform: uppercase;
    padding-bottom: 20px;
    letter-spacing: 5px;
    color: var(--dark-grayish-blue);
    font-weight: 100;
}

.content h2 {
    font-family: 'Fraunces', serif;
    font-size: 2.5rem;
    padding-bottom: 25px;
    color: var(--very-dark-blue);
}

.content p {
    font-family: 'Montserrat', sans-serif;
    color: var(--dark-grayish-blue);
    line-height: 25px;
    text-align: left;
    font-size: 1.15rem;
}

.content #prices {
    display: flex;
    padding: 25px 0;
    align-items: center;
}

.content #prices span:first-child {
    color: var(--dark-cyan);
    font-size: 2.5rem;
    font-family: 'Fraunces', serif;
    padding-right: 15px;
}

.content #prices span:last-child {
    color: var(--dark-grayish-blue);
    font-size: 1rem;
    font-family: 'Montserrat', serif;
    text-decoration: line-through;
}

.btn-icon {
    background-image: url("../assets/icon-cart.svg");
    background-size: cover;
    background-repeat: no-repeat;
    color: var(--white);
    margin-right: 10px;
}

.content button {
    display: flex;
    justify-content: center;
    background-color: var(--dark-cyan);
    font-family: 'Montserrat', sans-serif;
    width: 100%;
    padding: 15px 0;
    color: var(--white);
    border: none;
    border-radius: 7px;
    /* margin-left: 25%; */
}

.content button:hover {
    color: var(--white);
    background-color: var(--very-dark-blue);
    opacity: 0.95;
    cursor: pointer;
}

.attribution {
    font-size: 11px;
    text-align: center;
    margin-top: 15px;
}

.attribution a {
    color: hsl(228, 45%, 44%);
}

@media screen and (max-width: 400px) {

    .content {
        padding: 5%;
        text-align: left;
    }

    .card {
        display: grid;
        width: 350px;
        height: 600px;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr 1fr;
    }

    .image {
        width: 100%;
        border-top-right-radius: 10px;
        border-top-left-radius: 10px;
        border-bottom-left-radius: 0;
        background-position: center;
    }

    .content h1 {
        padding-bottom: 10px;
    }

    .content h2 {
        font-size: 2rem;
        padding-bottom: 15px;
        padding-right: 10px;
    }

    .content p {
        line-height: 25px;
        font-size: 1.07rem;
    }

    .content #prices {
        padding: 15px 0;
    }
}
</style>