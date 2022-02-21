<script lang="ts">
    import IDE from "./lib/IDE.svelte";
    import Notebooks from "./lib/Notebooks.svelte";
    import Team from "./lib/Team.svelte";
    import logo from "./assets/logo.png";

    const changePage = (page: string) => {
        let pages: string[] = ["home", "ide", "notebooks", "team"];

        pages.forEach((page_name) => {
            let to_remove = document.getElementById(page_name);
            to_remove.style.display = "none";
            console.log(page_name);
        });

        if (page === "home") {
            let page = document.getElementById("home");
            page.style.display = "flex";
        } else if (page === "ide") {
            let page = document.getElementById("ide");
            page.style.display = "flex";
        } else if (page === "notebooks") {
            let page = document.getElementById("notebooks");
            page.style.display = "flex";
        } else if (page === "team") {
            let page = document.getElementById("team");
            page.style.display = "flex";
        }
    };
</script>

<main>
    <section id="home">
        <h1>Code for Hope</h1>

        <button on:click|preventDefault={() => changePage("ide")}>IDE</button>
        <button on:click|preventDefault={() => changePage("notebooks")}>
            Notebooks
        </button>
        <button on:click|preventDefault={() => changePage("team")}>Team</button>

        <div class="tooltip">
            <a
                href="https://forms.gle/YGz6LpZn8FDsanHK8"
                target="_blank"
                class="link">VOLUNTEER</a
            >
            <span class="tooltiptext">Only for RI Y16 Students!</span>
        </div>

        <img src={logo} alt="Code for Hope Logo" />
    </section>

    <section class="page" id="ide">
        <IDE />
        <br />
        <button on:click|preventDefault={() => changePage("home")}>Home</button>
    </section>

    <section class="page" id="notebooks">
        <Notebooks />
        <br />
        <button on:click|preventDefault={() => changePage("home")}>Home</button>
    </section>

    <section class="page" id="team">
        <Team />
        <br />
        <button on:click|preventDefault={() => changePage("home")}>Home</button>
    </section>
</main>

<style>
    main {
        text-align: center;
        width: 100vw;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
    }

    h1 {
        color: #818cf8;
        font-size: 3rem;
    }

    button {
        border: none;
        border-radius: 0.5rem;
        background-color: #818cf8;
        cursor: pointer;
        transition: background-color 0.3s;
        width: 12rem;
        font-size: 1.5rem;
    }

    button:hover {
        background-color: #5968f8;
    }

    img {
        width: 5rem;
    }

    section {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        width: 100vw;
        height: 100vh;
    }

    .page {
        display: none;
    }

    .link {
        font-family: inherit;
        -webkit-padding: 0.4em 0;
        padding: 0.4em;
        margin: 0 0 0.5em 0;
        box-sizing: border-box;
        outline: none;
        color: #cbd5e1;
        text-decoration: none;
        border: none;
        border-radius: 0.5rem;
        background-color: #0ea5e9;
        cursor: pointer;
        transition: background-color 0.3s;
        width: 12rem;
        font-size: 1.5rem;
    }

    .link:hover {
        background-color: #0284c7;
    }

    .tooltip {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

    .tooltiptext {
        visibility: hidden;
        background-color: #0ea5e9;
        color: #fff;
        text-align: center;
        padding: 0.5rem 1rem;
        border-radius: 1rem;
        z-index: 1;
        text-align: center;
        font-size: 1rem;
    }

    .tooltip:hover .tooltiptext {
        visibility: visible;
    }

    @media (max-width: 640px) {
        h1 {
            font-size: 1.5rem;
        }

        button,
        .link {
            font-size: 1rem;
        }
    }
</style>
