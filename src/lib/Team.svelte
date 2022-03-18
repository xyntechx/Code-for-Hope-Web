<script lang="ts">
    import nyx from "../assets/nyx.jpg";
    import en_xing from "../assets/en-xing.jpg";
    import sohan from "../assets/sohan.jpg";
</script>

<main>
    <h1>The Core Team</h1>
    <p class="description">
        We are students of Raffles Institution (Class of 2022) on a mission to
        create a fair playing field independent of socio-economic status for all
        students, ultimately tackling income inequality. As programming is a 
        relevant and important skill in today's digital era, we hope that by
        introducing programming to young students, they will be equipped with
        the useful skill of programming and thus be better prepared for the future! 
        So far, we have recruited <span>25 volunteers</span>, collaborated with 
        <span>14 CDAC centres</span> and taught <span>200 students</span> in Singapore!
    </p>
    <section>
        <div>
            <img src={nyx} alt="Nyx Audrey Angelo Iskandar" />
            <p>Nyx Audrey Angelo Iskandar</p>
        </div>
        <div>
            <img src={en_xing} alt="Lao En Xing" />
            <p>Lao En Xing</p>
        </div>
        <div>
            <img src={sohan} alt="Sohan Daniel Singh" />
            <p>Sohan Daniel Singh</p>
        </div>
    </section>
</main>

<style>
    main {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
    }

    h1 {
        color: #818cf8;
        font-size: 3rem;
        margin: 0.5rem;
    }

    section {
        display: grid;
        column-gap: 2rem;
        grid-template-columns: repeat(3, 1fr);
        align-items: start;
        margin: 0 1rem;
        margin-top: 2rem;
    }

    div {
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
    }

    img {
        width: 10rem;
    }

    span {
        color: #818cf8;
    }

    .description {
        margin: 2rem 10rem;
        text-align: justify;
    }

    @media (max-width: 640px) {
        h1 {
            font-size: 1.5rem;
        }

        img {
            width: 5rem;
        }

        section {
            column-gap: 1rem;
            margin-top: 1rem;
        }

        .description {
            margin: 1rem 2rem;
            font-size: 0.7rem;
        }
    }
</style>
