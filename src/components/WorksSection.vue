<template>
    <div class="works">
        <div class="header">
            <div class="topTitle">
                <div class="divider"></div>
                <h5 class="">Project that our clients love</h5>
            </div>
            <div class="mainTitle">
                <h3>Works</h3>
                <a class="allProjectsBtn" href="/">Explore all projects &#129130;</a>
            </div>
        </div>
        <div class="articles">
            <div class="column">
                <div class="item">
                    <div class="image googleArtsCulture"></div>
                    <div class="content">
                        <h4>Google Art & Culture</h4>
                        <p>Exploring new upcoming features in Google arts and culture and its future enhancement</p>
                    </div>
                </div>
                <div class="item">
                    <div class="image eBank"></div>
                    <div class="content">
                        <h4>E - bank</h4>
                        <p>Exploring new upcoming features in Google arts and culture and its future enhancement</p>
                    </div>
                </div>
            </div>
            <div class="column">
                <div class="item">
                    <div class="image abstractIllustration"></div>
                    <div class="content">
                        <h4>Abstract illustration</h4>
                        <p>Engaging online class with interaction between masters and students and offering more valueable features</p>
                    </div>
                </div>
                <div class="item">
                    <div class="image tutorApplication"></div>
                    <div class="content">
                        <h4>Tutor application</h4>
                        <p>Engaging online class with interaction between masters and students and offering more valueable features</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .header {
        .topTitle {
            .divider {
                display: inline-block;
                border-bottom: 3px var(--primary-color) solid;
                width: 30px;
                vertical-align: middle;
                margin-right: 2rem;
            }
            h5 {
                display: inline-block;
            }
        }
        .mainTitle {
            display: flex;
            flex-direction: column;
            padding: 2rem 0;

            @media only screen and (min-width: 768px) {
                padding: 4rem 0;
            }
            .allProjectsBtn {
                margin-left: unset;
            }
            @media only screen and (min-width: 576px) {
                flex-direction: row;
                
                .allProjectsBtn {
                    margin-left: auto;
                    align-self: center;
                }
            }
        }
    }
    .articles {
        display: flex;
        gap: 0;
        flex-wrap: wrap;
        justify-content: center;

        @media only screen and (min-width: 768px) {
            flex-wrap: nowrap;
            gap: 4rem;
        }

        .column {
            width: 100%;

            .item {
                margin-bottom: 2rem;
                
                @media only screen and (min-width: 768px) {
                    margin-bottom: 4rem;
                }
                .image {
                    width: 100%;
                    background-repeat: no-repeat;
                    background-position: center;
                    background-size: cover;
                    margin-bottom: 1rem;

                    @media only screen and (min-width: 768px) {
                        margin-bottom: 2rem;
                    }


                    &.googleArtsCulture {
                        aspect-ratio: 5/8;
                        background-image: url("../assets/img/cave.jpg");
                    }
                    &.eBank {
                        aspect-ratio: 1;
                        background-image: url("../assets/img/E-bank.jpg");
                    }
                    &.abstractIllustration {
                        aspect-ratio: 1;
                        background-image: url("../assets/img/Abstract.jpg");
                    }
                    &.tutorApplication {
                        aspect-ratio: 5/8;
                        background-image: url("../assets/img/Phone.jpg");
                    }
                }
                .content {
                    h3 {
                        font-size: 2rem;
                    }
                    p {
                        margin: 1rem 0 0;
                        color: var(--tertiary-color);
                        width: 100%;

                        @media only screen and (min-width: 586px) {
                            width: 80%;
                        }
                    }
                }
            }
        }
    }
</style>