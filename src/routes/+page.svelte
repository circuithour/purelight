<main>
    <div class="header">
        <nav id="header-nav">
            <a href="/">
                <svg
                    id="logo"
                    width="55"
                    height="55"
                    viewBox="0 0 55 55"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                >
                    <path
                        d="M1.98441 29.2899C1.98441 27.0299 2.42954 24.7919 3.29444 22.704C4.15935 20.6159 5.42701 18.7187 7.02513 17.1206C8.62324 15.5225 10.5204 14.2548 12.6084 13.3899C14.6965 12.5251 16.9344 12.0799 19.1945 12.0799V29.2899H1.98441Z"
                        class="ccustom"
                        fill="#ffffff"
                        stop-color="#ffffff"
                    />
                    <path
                        d="M1.98441 29.2899C1.98441 31.55 2.42954 33.7879 3.29444 35.876C4.15935 37.964 5.42701 39.8612 7.02513 41.4593C8.62324 43.0574 10.5204 44.3251 12.6084 45.19C14.6965 46.0549 16.9344 46.5 19.1945 46.5V29.2899H1.98441Z"
                        class="ccompli1"
                        fill="#ffffff"
                        stop-color="#ffffff"
                    />
                    <path
                        d="M36.4043 29.2899C36.4043 31.55 35.9595 33.7879 35.0947 35.876C34.2298 37.964 32.9622 39.8612 31.3638 41.4593C29.7657 43.0574 27.8685 44.3251 25.7804 45.19C23.6925 46.0549 21.4545 46.5 19.1945 46.5V29.2899H36.4043Z"
                        class="ccompli2"
                        fill="#ffffff"
                        stop-color="#ffffff"
                    />
                    <path
                        d="M47.0156 14.422C47.0156 21.5586 41.23 27.344 34.0935 27.344H21.1716V14.422C21.1716 7.2854 26.957 1.5 34.0935 1.5C41.23 1.5 47.0156 7.2854 47.0156 14.422Z"
                        class="ccustom"
                        fill="#ffffff"
                        stop-color="#ffffff"
                    />
                </svg>
            </a>
            <a href="/Red">Red</a>
            <a href="/Green">Green</a>
            <a href="/Blue">Blue</a>
            <a href="/Bitch">Bitch</a>
        </nav>
    </div>

    <div class="container">
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
        left: 0;
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
        width: 30%;
        margin: auto;
    }

    .container {
        background-color: #03031f25;
        border-radius: 15px;
        padding: 0.25rem;
        height: auto;
        width: 650px;
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
        color: white;
        text-decoration: none;
        font-family: sans-serif;
        transition: color 0.5s linear;
    }

    a:hover {
        color: rgb(95, 184, 224);
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
        position: absolute;
    }
</style>
