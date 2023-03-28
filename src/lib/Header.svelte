<body>
    <nav class="grid">
        <a class="home" href="/">home</a>
        <a class="info" href="/info">info</a>
    </nav>
</body>

<style>
    a {
        color: black;
        text-decoration:underline;
        font-size: 1.2rem;
    }
    a:hover { 
        color: rgb(210, 204, 204);
    }

    a:visited {
        text-decoration: none;
    }

    nav a {
        font-size: 3rem;
    }
    nav {
        grid-template-columns: 7fr 1fr 1fr 1fr;
        justify-items: center;
        grid-template-areas:
        ". home info .";
        margin: 3rem 0px;
    }

    .home {
        grid-area: home;
    }
    .info {
        grid-area: info;
    }

    .grid {
        display: grid;
    }
</style>