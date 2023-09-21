<template>
    <div class="specialisation">
        <div class="header">
            <div class="topTitle">
                <div class="divider"></div>
                <h5>What I do best</h5>
            </div>
            <h3 class="mainTitle">Specialisation</h3>
        </div>
        <div class="items">
            <div class="item">
                <div class="image"></div>
                <h4 class="title">Product Design</h4>
            </div>
            <div class="item">
                <div class="image"></div>
                <h4 class="title">Branding</h4>
            </div>
            <div class="item">
                <div class="image"></div>
                <h4 class="title">Illustration</h4>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .specialisation {
        margin-bottom: 4rem;

        @media only screen and (min-width: 768px) {
            margin-bottom: 6rem;
        }
        
    }
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
            padding: 2rem 0;

            @media only screen and (min-width: 768px) {
                padding: 4rem 0;
            }

        }
    }
    .items {
        display: flex;
        flex-direction: column;
        width: 100%;
        justify-content: space-between;
        align-items: center;
        gap: 2rem;

        @media only screen and (min-width: 992px) {
            flex-direction: row;
        }
        @media only screen and (min-width: 768px) {
            gap: 3rem;
        }
        
        .item {
            width: 100%;
            max-width: 500px;

            @media only screen and (min-width: 1200px) {
                width: 33%;
            }

            .image {
                aspect-ratio: 4/3;
                background-repeat: no-repeat;
                background-position: center;
                background-size: cover;
                width: 100%;
                margin-bottom: 1rem;

                @media only screen and (min-width: 768px) {
                    margin-bottom: 2rem;
                }
                
            }
            &:nth-child(1) {
                .image {
                    background-image: url('../assets/img/Glasses-thrown.jpeg');
                }
            }
            &:nth-child(2) {
                .image {
                    background-image: url('../assets/img/Plant.jpeg');
                }
            }
            &:nth-child(3) {
                .image {
                    background-image: url('../assets/img/Angy-man.jpg');
                }
            }
        }
    }
</style>