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

        <div class="link-box"><a href="/Cal">Planner</a></div>
        <div class="link-box"><a href="/Green">Green</a></div>
        <div class="link-box"><a href="/Blue">Blue</a></div>
        <div class="link-box"><a href="/Bitch">Bitch</a></div>
    </nav>
</div>

<style>
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
</style>
