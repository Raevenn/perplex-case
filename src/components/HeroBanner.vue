<script setup>
</script>

<template>
    <div class="hero">
        <div class="textContent">
            <h4>Sakura Haruno</h4>
            <!-- Naruto fans I see -->
            <h2 class="mainTitle">Designer & Illustrator</h2>
            <p class="subtitle">Norway based designer who specialised in Product design and Illustration.</p>
        </div>
        <div class="image">
            <img src="../assets/img/Person.jpg" alt="person">
        </div>
    </div>
</template>

<style lang="scss" scoped>
    h1, h2, h3 {
        margin: 0;
    }
    .hero {
        display: flex;
    }
    .textContent {
        display: flex;
        flex-direction: column;
        justify-content: center;
        width: 40%;

        .mainTitle {
            // TODO: make bigger and cause overlap
            padding: 1rem 0 2rem;
            font-size: 5rem;
            font-weight: 800;
        }
        .subtitle {
            color: var(--tertiary-color);
            font-weight: 600;
        }
    }
    .image {
        width: 60%;

        img {
            width: 100%;
            aspect-ratio: 1;
        }
    }
</style>