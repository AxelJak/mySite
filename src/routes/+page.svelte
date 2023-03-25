<body>
    <nav class="grid">
        <a class="home" href="/">home</a>
        <a class="info" href="/info">info</a>
    </nav>
    
    <div class="grid container">
        <h4 class="intro" >hello my name is <br> &nbsp;&nbsp;&nbsp;&nbsp; Axel Jakobsson</h4>
        <h4 class="web-developer" >i'm a web developer</h4>
        <img class="norge" src="norge.jpg" alt="Axel in Norway">
        <img class="blabar" src="blabar.jpg" alt="Axel eating blueberries">
        <h4 class="umea">based in umeå</h4>
        <a class="my_work" href="my_work.hmtl">my work</a>
        
    </div>
    <footer class="grid">
        <h5 class="contact">contact - <br> axel.jakobsson3@gmail.com</h5>
    </footer>
</body>

<style>
    * {
    background-color: white;
    font-family: monospace, sans-serif;
    }

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

    .container {
        grid-template-columns: auto auto;
        place-items: center;
        grid-template-areas: 
        "intro bar"
        "web bar"
        "norge bar" 

        "norge work"
        "norge umea";

    }

    h4 {
        font-size: 1.2rem;
        font-weight: 300;
    }

    .blabar {
        grid-area: bar;
    }

    .norge {
        grid-area: norge;
    }

    .intro {
        grid-area: intro;
    }

    .web-developer {
        grid-area: web;
    }

    .my_work {
        grid-area: work;
    }

    .umea {
        grid-area: umea;
    }

    img {
        padding: 2rem;
        width: 30rem;
    }

    footer {
        justify-items: center;
    }
</style>