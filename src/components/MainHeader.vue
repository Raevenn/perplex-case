<template>
    <head>
        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
        <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;700;800&display=swap" rel="stylesheet">
    </head>

    <header>
        <div class="headerBar">
            <div class="logo">
                <img src="../assets/img/Logo.png" alt="haruno-logo">
            </div>
            <div class="title">
                <b>HARUNO</b>
            </div>
            <div class="break"></div>
            <div class="items">
                <a href="/" class="item">Works</a>
                <a href="/" class="item">About</a>
                <a href="/" class="item">Media</a>
                <a href="/" class="item">Contact</a>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
.headerBar {
    display: flex;
    flex: 0 0 100%;
    flex-direction: row;
    align-items: center;
    width: 100%;
    padding-bottom: 2rem;
    flex-wrap: wrap;
    
    @media only screen and (min-width: 768px) {
        flex-wrap: nowrap;
    }

    .logo {
        aspect-ratio: 1;
        padding-right: 1rem;
    }
    .title {
        width: 50%;
        align-self: center;
    }
    .items {
        display: flex;
        flex-direction: row;
        justify-content: end;
        width: 100%;
        flex-wrap: wrap;
        
        @media only screen and (min-width: 578px) {
            flex-wrap: nowrap;
        }
        @media only screen and (min-width: 992px) {
            width: 50%;
        }
        .item {
            padding: 0.5rem 1rem;
            margin: 0 1rem;

            @media only screen and (max-width: 767px) {
                // padding: 0.5rem 0.5rem;
                // margin: 0 0.5rem;
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

        @media only screen and (min-width: 992px) {
            display: none;
        }
    }
}
</style>