<main>
    <section>
        <h1>Day 1</h1>
        <div class="box">
            <section class="links">
                <a
                    href="https://colab.research.google.com/drive/12465FAGnWeJEUiKQ3fQTt7o2d9VamAxm"
                    target="_blank">Lesson 1</a
                >
                <a
                    href="https://colab.research.google.com/drive/1norfrupFiycu1krAZA6rhFvbIWWBhnTP"
                    target="_blank">Practice 1</a
                >
            </section>

            <p>What is programming?</p>
            <p>What is Python?</p>
            <p>What can I do with Python?</p>
        </div>

        <br />

        <div class="box">
            <section class="links">
                <a
                    href="https://colab.research.google.com/drive/1tO2ah9TvT120n17FmKm03RL5rE_DOQPs"
                    target="_blank">Lesson 2</a
                >
                <a
                    href="https://colab.research.google.com/drive/1ZbLiaePfaNhGdwxcfufkNAx6ElYX2wpf"
                    target="_blank">Practice 2</a
                >
            </section>

            <p>What can I do with strings?</p>
            <p>What are conditionals?</p>
            <p>What are loops?</p>
        </div>
    </section>

    <section>
        <h1>Day 2</h1>
        <div class="box">
            <section class="links">
                <a
                    href="https://colab.research.google.com/drive/1lhsAyANIh8aAF73LN2It05PL4oqJxIfu"
                    target="_blank">Lesson 3</a
                >
                <a
                    href="https://colab.research.google.com/drive/1om6iIe9k6hyMQSmRJqVsKInl-B8593hM"
                    target="_blank">Practice 3</a
                >
            </section>

            <p>What are functions?</p>
            <p>What are tuples and lists?</p>
            <p>What are dictionaries?</p>
        </div>

        <br />

        <div class="box">
            <section class="links">
                <a
                    href="https://colab.research.google.com/drive/1cjJDJgy8wsA1hfyYe_gmTzwayXwi7bp4"
                    target="_blank">Lesson 4</a
                >
                <a
                    href="https://colab.research.google.com/drive/14jVCt9MnNB3Cgld91tNW8dKzcAF4Cw3M"
                    target="_blank">Practice 4</a
                >
            </section>

            <p>What is Object Oriented Programming (OOP)?</p>
            <p>What are classes?</p>
            <p>What is inheritance?</p>
        </div>
    </section>
</main>

<style>
    main {
        display: grid;
        column-gap: 2rem;
        grid-template-columns: repeat(2, minmax(0, 1fr));
        font-size: 1.5rem;
        margin: 0 1rem;
    }

    h1 {
        color: #818cf8;
        font-size: 3rem;
        margin: 0.5rem;
    }

    p {
        margin: 1rem;
    }

    a {
        border: none;
        border-radius: 0.5rem;
        background-color: #818cf8;
        cursor: pointer;
        transition: background-color 0.3s;
        color: #cbd5e1;
        width: 7rem;
        text-decoration: none;
        padding: 0.5rem 0;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    a:hover {
        background-color: #5968f8;
    }

    .links {
        display: flex;
        justify-content: center;
        align-self: center;
        column-gap: 2rem;
        margin-top: 1.5rem;
    }

    .box {
        border: 0.1rem solid white;
        padding: 0 0.2rem;
    }

    @media (max-width: 640px) {
        main {
            font-size: 0.8rem;
            column-gap: 1rem;
        }

        h1 {
            font-size: 1.5rem;
        }

        .links {
            margin-top: 1rem;
            column-gap: 1rem;
        }

        a {
            padding: 0.2rem;
        }
    }
</style>
