<script>
    import Header from "$lib/Header.svelte";
    import Footer from "$lib/Footer.svelte";

</script>
<body>
    <Header/>

    <div class="box flex">
        
        <div class="work flex">
            <h1>XLENT</h1>
            <p>Right now I work at XLENT as a web developer.</p>
        </div>

        <div class="work flex">
            <h1>BAE Systems Hägglunds</h1>
            <p>I worked two summers at BAE Systems Hägglunds as a system developer. Developing tools 
                that made the internal processes more efficient. We used python to build applications.
            </p>
        </div>

        <div class="work flex">
            <h1>Övik lunch redesign</h1>
            <h2>My design: <a href="https://wondrous-parfait-4e37b1.netlify.app/">My version</a></h2>
            <h2>Original design: <a href="https://lunch.ovik.info/">Original Site</a></h2>
            <p>
                Övik has a lunch resturantwebiste that keeps track of the lunch menus in the city. I didn't like the design of the website so I decided to redesign it. 
            </p>
        </div>
        
    </div>

    <Footer/>
    
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

    .flex {
        display: flex;
    }

    .box {
        flex-wrap: wrap;
        justify-content: center;
    }

    .work {
        justify-items: center;
        align-items: center;
        flex-wrap: wrap;
        border: 1px solid black;
        width: 50%;
    }

</style>