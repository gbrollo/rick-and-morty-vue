<<template>
    <div class="home">
        <div class="logo">
            <img style="max-width: 100%" src="src/assets/rick_and_morty.png" alt="Rick and Morty" />
        </div>
        <div class="text">
        <p>
            Rick and Morty is an American adult animated science fiction sitcom created by Justin Roiland and Dan Harmon for Cartoon Network's nighttime programming block, Adult Swim. The series follows the misadventures of cynical mad scientist Rick Sanchez and his good-hearted, but fretful grandson Morty Smith, who split their time between domestic life and interdimensional adventures.

            Roiland voices the eponymous characters, with Chris Parnell, Spencer Grammer and Sarah Chalke voicing the rest of Rick and Morty's family. The series originated from an animated short parody film of Back to the Future, created by Roiland for Channel 101, a short film festival co-founded by Harmon. The series has been acclaimed by critics for its originality, creativity and humor.

            The fifth season premiered on June 20, 2021, and consisted of ten episodes. A sixth season was confirmed as part of a long-term deal in May 2018 that ordered 70 new episodes over an unspecified number of seasons.
        </p>
        </div>
    </div>
</template>

<script>
export default {
}
</script>

<style type="text/css">
    .home {
        width: 100%;
        text-align: center;
    }
    .logo {
        width: 100%;
        display: table;
        margin: 0 auto;
    }
    .text p {
        text-align: left;
        color: #fff;
        font-size: 1.4rem;
        margin: 20px;
        font-family: Helvetica, sans-serif;
        word-spacing: 6px;
        text-indent: 1cm;
        letter-spacing: 1px;
        line-height: 36px;
        text-shadow: 4px 4px 2px black;
    }
    /* Extra small devices (phones, 600px and down) */
    @media only screen and (max-width: 600px) {}

    /* Small devices (portrait tablets and large phones, 600px and up) */
    @media only screen and (min-width: 600px) {
        .logo {
            width: 80%;
        }
        .text p {
            text-align: justify;
        }
    }

    /* Medium devices (landscape tablets, 768px and up) */
    @media only screen and (min-width: 768px) {
        .logo {
            width: 50%;
        }
    }

    /* Large devices (laptops/desktops, 992px and up) */
    @media only screen and (min-width: 992px) {
        .logo {
            width: 40%;
        }
    }

    /* Extra large devices (large laptops and desktops, 1200px and up) */
    @media only screen and (min-width: 1200px) {
        .logo {
            width: 30%;
        }
    }
</style>
