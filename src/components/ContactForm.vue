<template>
    <div class="contactForm">
        <div class="header">
            <h3>Let's connect</h3>
            <p>Got a project? Feel free to get in touch</p>
            <a href="mailto:sakura@haruno.com">sakura@haruno.com</a>
        </div>

        <form action="/">
            <input type="text" placeholder="Your sweet name" class="name">
            <input type="text" placeholder="your email address" class="email">
            <textarea  type="textarea" placeholder="About your message" class="message" />
            <button type="submit">SEND <br> &#129130;</button>
        </form>
    </div>
</template>

<style lang="scss" scoped>
    .contactForm {
        margin-top: 2rem;
    }
    .contactForm .header {
        text-align: center;
        margin-bottom: 4rem;

        p {
            color: var(--tertiary-color);
        }
        a {
            color: var(--accent-color);
        }
    }
    form {
        width: 100%;
        margin: 0 auto;
        display: flex;
        flex-direction: column;
        gap: 2rem;
        flex-wrap: wrap;
        
        @media only screen and (min-width: 992px) {
            width: 70%;
            flex-direction: row;
        }

        input, textarea {
            border: none;

            &:focus {
                border-color: var(--primary-color);
            }
        }
        .name {
            flex-basis: 100%;
            flex-grow: 1;
            padding: 2rem;
            @media only screen and (min-width: 992px) {
                flex-basis: 20%;
            }

        }
        .email {
            flex-basis: 100%;
            flex-grow: 1;
            padding: 2rem;
            @media only screen and (min-width: 992px) {
                flex-basis: 20%;
            }

        }
        .message {
            flex-basis: 100%;
            flex-grow: 8;
            padding: 2rem;
            @media only screen and (min-width: 992px) {
                flex-basis: 60%;
            }

        }
        button {
            background-color: #62ba55;
            color: #fff;
            font-size: 1rem;
            border: none;
            flex-grow: 1;
            width: 100px;
            aspect-ratio: 1;
            align-self: flex-end;

            @media only screen and (min-width: 992) {
                width: 20%;
            }
        }
    }
</style>