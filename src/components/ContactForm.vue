<template>
    <div class="contactForm">
        <h2>Let's connect</h2>
        <p>Got a project feel free to get in touch</p>
        <a href="mailto:sakura@haruno.com">sakura@haruno.com</a>

        <form action="/">
            <input type="text" placeholder="Your sweet name" class="name">
            <input type="text" placeholder="your email address" class="email">
            <input type="text" placeholder="About your message" class="message">
            <button type="submit">Send</button>
        </form>
    </div>
</template>

<style lang="scss" scoped>
    form {
        width: 70%;
        margin: 0 auto;
        display: flex;
        flex-direction: row;
        gap: 2rem;
        flex-wrap: wrap;
+
        .name {
            flex-basis: 40%;
            flex-grow: 1;
            padding: 2rem;
        }
        .email {
            flex-basis: 40%;
            flex-grow: 1;
            padding: 2rem;
        }
        .message {
            flex-basis: 60%;
            flex-grow: 8;
            padding: 2rem;
        }
        button {
            background-color: #62ba55;
            color: #fff;
            font-size: 2rem; 
            border: none;
            flex-grow: 1;
            width: 20%;
            aspect-ratio: 1;
        }
    }
</style>