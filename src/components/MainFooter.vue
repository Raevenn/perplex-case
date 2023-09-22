<template>
    <footer>
        <div class="footer">
            <div class="logo">
                <img src="../assets/img/Logo.png" alt="haruno-logo">
            </div>
            <div class="items">
                <a href="/" class="item">Works</a>
                <a href="/" class="item">About</a>
                <a href="/" class="item">Media</a>
            </div>
            <div class="break"></div>
            <!-- TODO: make social icons -->
            <div class="items socials">
                <a href="/" class="item">Bê</a>
                <a href="/" class="item">Web</a>
                <a href="/" class="item">LinkedIn</a>
                <a href="/" class="item">Twitter</a>
                <a href="/" class="item">Instagram</a>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
.footer {
    display: flex;
    flex: 0 0 100%;
    flex-direction: row;
    align-items: center;
    width: 100%;
    padding-bottom: 2rem;
    margin-top: 10rem;
    flex-wrap: wrap;
    
    @media only screen and (min-width: 1200px) {
        flex-wrap: nowrap;
    }
    .logo {
        aspect-ratio: 1;
        padding-right: 1rem;
    }
    .items {
        display: flex;
        flex-direction: row;
        width: auto;
        flex-wrap: wrap;

        @media only screen and (min-width: 1200px) {
            width: 50%;
            flex-wrap: nowrap;
        }
        &.socials {
            justify-content: end;
            width: 100%;
            .item {
                margin: 0 0.5rem;
            }
        }
        .item {
            padding: 0.5rem 1rem;
            margin: 0 1rem;

            @media only screen and (max-width: 767px) {
                margin: 0 0.5rem;
                font-size: 0.8rem;
            }
            &:last-child {
                margin-right: 0;
            }
        }
    }
    .break {
        flex-basis: 100%;
        height: 0;

        @media only screen and (min-width: 1200px) {
            display: none;
        }
    }
}
</style>