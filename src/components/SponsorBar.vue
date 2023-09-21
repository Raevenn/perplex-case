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
        margin: 8rem 0;
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        align-items: center;
        width: 100%;
        gap: 1rem;
        flex-wrap: wrap;

        @media only screen and (min-width: 900px ) {
            flex-wrap: nowrap;
        }

        .logo {

        }
    }
</style>