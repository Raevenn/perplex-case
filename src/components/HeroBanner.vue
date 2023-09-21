<script setup>
</script>

<template>
    <div class="hero">
        <div class="textContent">
            <div class="floatingContainer">
                <h4 class="nameTitle">Sakura Haruno</h4>
                <!-- Naruto fans I see -->
                <h2 class="mainTitle">Designer & Illustrator</h2>
                <p class="subtitle">Norway based designer who specialised in Product design and Illustration.</p>
            </div>
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
        position: relative;
        flex-direction: column;
        
        @media only screen and (min-width: 992px) {
            flex-direction: row;
        }
    }
    .textContent {
        width: 100%;

        @media only screen and (min-width: 992px) {
            width: 0;
        }
        @media only screen and (min-width: 1200px) {
            width: 40%;
        }
        .floatingContainer {
            width: 100%;
            z-index: 9;
            order: 2;

            @media only screen and (min-width: 992px) {
                display: flex;
                flex-direction: column;
                justify-content: center;
                position: absolute;
                left: 0;
                top: 50%;
                transform: translate(0,-50%);
                order: 1;
            }
            @media only screen and (min-width: 1200px) {
                width: 40%;
            }

            .nameTitle {
                @media only screen and (min-width: 1200px) {
                    padding-bottom: 20rem;
                }
            }
            .mainTitle {
                position: block;
                padding: 1rem 0 2rem;
                width: 100%;

                @media only screen and (min-width: 1200px) {
                    width: 140%;
                    position: absolute;
                }
                
            }
            .subtitle {
                margin: 0;
                color: var(--tertiary-color);
                font-weight: 600;
            }
        }
    }
    .image {
        width: 100%;
        order: -1;

        @media only screen and (min-width: 1200px) {
            width: 60%;
            order: 2;
        }

        img {
            width: 100%;
            aspect-ratio: 1;
        }
    }
</style>