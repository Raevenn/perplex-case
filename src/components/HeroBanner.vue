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
            <div class="miniCard">
                <a href="/">About Myself <span style="margin-left: 1rem">&#129130;</span></a>
            </div>
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
                font-family: 'Dancing Script', cursive;
                font-weight: 700;
                font-size: 1.5rem;
                
                @media only screen and (min-width: 768px) {
                    font-size: 3rem;
                }
                @media only screen and (min-width: 1200px) {
                    padding-bottom: 20rem;
                }
            }
            .mainTitle {
                position: block;
                padding: 1rem 0;
                width: 100%;

                // transparant image text effect
                background-image: url("../assets/img/paint.jpg");
                background-repeat: repeat;
                background-size: contain;
                -webkit-background-clip: text;
                -webkit-text-fill-color: transparent;

                @media only screen and (min-width: 1200px) {
                    padding: 1rem 0 2rem;
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
        position: relative;
        width: 100%;
        order: -1;

        @media only screen and (min-width: 1200px) {
            width: 60%;
            order: 2;
        }
        .miniCard {
            position: absolute;
            right: 0;
            bottom: 0;
            padding: 1rem 0.5rem;
            background-color: white;
            font-size: 1rem;
            font-weight: 500;

            @media only screen and (min-width: 576px) {
                padding: 2rem 1rem;
                font-size: 1.5rem;
            }

            a {
                padding: 1rem;
            }
        }
        img {
            width: 100%;
            aspect-ratio: 1;
        }
    }
</style>