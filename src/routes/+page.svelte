<script>
    import Footer from "$lib/Footer.svelte";
    import Header from "$lib/Header.svelte";

</script>
<body>
    
    <Header/>
    <div class="container">

        <h4 class="intro" >hello my name is <br> &nbsp;&nbsp;&nbsp;&nbsp; Axel Jakobsson</h4>
        <h4 class="web-developer" >i'm a web developer</h4>
        <img class="norge" src="norge.jpg" alt="Axel in Norway">
        <img class="blabar" src="blabar.jpg" alt="Axel eating blueberries">
        <h4 class="umea">based in umeå</h4>
        <a class="my_work" href="/myWork">my work</a>
    
        <Footer/>
    </div>

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

    .container {
        display: grid;
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

    @media only screen and (max-width: 600px) {
        .container {
            display: flex;
            flex-direction: column;
            justify-content: center;
        }
        img {
            padding: 2rem;
            width: 70%;
        }
    }
    img {
        padding: 2rem;
        width: 30rem;
    }
</style>