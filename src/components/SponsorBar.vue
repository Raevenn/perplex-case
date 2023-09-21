<template>
    <div class="sponsorBar">
        <div class="logo">
            <img src="../assets/img/GoogleLogo.png" alt="google-logo">
        </div>
        <div class="logo">
            <img src="../assets/img/FlickrLogo.png" alt="flick-logo">
        </div>
        <div class="break"></div>
        <div class="logo">
            <img src="../assets/img/Natgeologo.png" alt="nat-geo-logo">
        </div>
        <div class="logo">
            <img src="../assets/img/Slack.png" alt="slack-logo">
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .sponsorBar {
        margin: 4rem 0;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        width: 100%;
        gap: 2rem;
        flex-wrap: wrap;
        max-width: 100%;

        @media only screen and (min-width: 992px ) {
            flex-wrap: nowrap;
            margin: 8rem 0;
        }

        .logo {
            text-align: center;
            flex-grow: 1;

            @media only screen and (min-width: 992px ) {
                flex-grow: 3;
                text-align: start;
            }
            img {
                max-width: 200px;
                background-repeat: no-repeat;
                background-position: center;
                background-size: cover;
                max-height: 100px;
            }
            &:last-child {
                flex-grow: 1;
                text-align: center;

                @media only screen and (min-width: 992px ) {
                    text-align: end;
                }

            }
        }
        .break {
            flex-basis: 100%;
            height: 0;

            @media only screen and (min-width: 992px ) {
                display: none;
            }
        }
    }
</style>