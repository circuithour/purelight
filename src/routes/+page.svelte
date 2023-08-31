<script>
    import Header from "../lib/Header.svelte";
</script>

<main>
    <Header />

    <div class="container" id="calltocontainer">
        <div id="callto">
            <span id="cum"
                ><p>You can purchase a brand new Overwatch Winton for only</p>
                <p class="important">$12.99</p>
                <p>Act Fast, Act Now</p>
            </span>
            <button id="buy">Buy Now</button>
        </div>
    </div>

    <div class="container">
        <div id="callto2">
            <span id="cum"
                ><p>You can purchase a second Overwatch Winton for only</p>
                <p class="important">$6.99</p>
                <p>Wow!!!!</p>
            </span>
            <button id="buy">Buy Now</button>
        </div>
    </div>
</main>

<style>
    h1 {
        font-size: 200%;
        color: blue;
        font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI",
            Roboto, Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue",
            sans-serif;
    }

    .header {
        position: sticky;
        display: flex;
        top: 0;
        margin: 0;
        height: 55px;
        width: 100svw;
        background-color: #071023;
        flex-direction: row;
        justify-content: center;
        gap: 2rem;
    }

    #header-nav {
        display: flex;
        color: white;
        justify-content: space-evenly;
        margin: auto;
        gap: 1rem;
    }

    .container {
        border: solid 1px rgba(0, 0, 0, 0.144);
        background-color: #03031f25;
        border-radius: 15px;
        padding: 1rem;
        height: auto;
        width: auto;
        display: flex;
        justify-content: center;
        text-align: center;
        margin: auto;
    }

    #callto {
        font-size: 2rem;
        display: flex;
        flex-direction: column;
        text-align: center;
        font-family: Arial, Helvetica, sans-serif;
    }

    #calltocontainer {
        margin-top: 80px;
    }

    .link-box {
        border-radius: 8px;
        width: 80px;
        height: 35px;
        display: flex;
        gap: 1rem;
        justify-content: center;
        transition: all 0.1s linear;
    }

    .link-box:hover {
        background-color: #0e2046;
        transition: all 0.1s linear;
        cursor: pointer;
    }

    #callto2 {
        font-size: 2rem;
        display: flex;
        flex-direction: column;
        text-align: center;
        font-family: Arial, Helvetica, sans-serif;
    }

    #buy {
        border: solid 1px rgba(32, 110, 62, 0.521);
        background-color: rgb(94, 218, 150);
        color: white;
        border-radius: 8.5px;
        margin: 1rem auto;
        font-weight: bold;
        padding: 0.5rem;
        width: 120px;
        transition: all 0.2s ease-out;
    }

    #buy:hover {
        background-color: rgb(68, 165, 112);
        transition: all 0.2s ease-out;
    }

    #buy:active {
        transform: translateY(2px);
    }

    #cum {
        margin: 2.5rem 1rem 1rem 0rem;
        line-height: 3rem;
    }

    .important {
        font-weight: bold;
    }

    p {
        margin: 0;
    }

    a,
    a:visited {
        margin: auto;
        color: white;
        text-decoration: none;
        font-family: sans-serif;
        transition: color 0.5s linear;
    }

    #logo {
        position: absolute;
        display: inline-block;
        left: 1.5rem;
        top: 0;
        padding: 3px 0;
        transition: color 0.5s linear;
    }

    #logo:hover {
        fill: rgb(95, 184, 224);
        transition: color 0.5s linear;
    }

    main {
        display: flex;
        flex-direction: column;
        gap: 20rem;
        margin: 0;
        padding: 0;
        left: 0;
    }
</style>
