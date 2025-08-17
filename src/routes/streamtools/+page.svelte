<script>
	import StreamToolsNavbar from "$lib/components/StreamToolsNavbar.svelte";

    let games = [
        {
            name: "SRN Feud",
            description: "Host Google Feud for your viewers to play!",
            image: "/project_images/srn_feud.png",
            download: "https://chromewebstore.google.com/detail/srn-feud/koonghjejgkkfjbhplbkbbknhnhlogki",
            demo: "https://youtu.be/YeO-S66FwSk"
        },
        {
            name: "Epic Contexto",
            description: "Play Contexto",
            image: "/project_images/srn_feud.png",
            download: "https://chromewebstore.google.com/detail/epic-contexto/ogajjnifdkiolcgoahhphdhgeejeahmm"
        }
    ];
</script>

<title>Stream Tools - SRN's Site</title>
<StreamToolsNavbar />

<main>
	<div class="hero">
        <h2>Stream Tools</h2>
        <h5>Fun interactive games that engage your audience, <span class="free">for free</span>.</h5>
    </div>

    <div class="games text-center d-flex justify-content-center align-items-center flex-column p-4">
        <h3>Games</h3>
        <p class="mb-3">Games you can play with your viewers!</p>

        <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 row-cols-lg-4 gap-4 d-flex justify-content-center align-items-center">
            {#each games as game}
                <div class="card" style="width: 18rem; height: 100%; min-height: 100%;">
                    <img src="{game.image}" class="card-img-top" alt="{game.name}">
                    <div class="card-body" style="background-color: #202124;">
                        <h5 class="card-title mb-3">{game.name}</h5>
                        <!-- <p class="card-text">{game.description}</p> -->
                        {#if game.download}
                            <a href="{game.download}" target="_none" class="btn btn-success {game.demo ? "me-3" : ""}">Download</a>
                        {/if}
                        {#if game.demo}
                            <a href="{game.demo}" target="_none" class="btn btn-outline-success">Demo</a>
                        {/if}
                    </div>
                </div>
            {/each}
        </div>
    </div>
</main>

<style>
	:root, main {
		background-color: #1a1a1a;
        color: white;
        margin: 0;
        padding: 0;
        flex-direction: column;
	}

    .free {
        text-decoration: underline;
        color: lime;
    }

    .hero {
        width: 100%;
        height: 60vh;
        background: #0088ff;
        background: linear-gradient(155deg, #8009ff 0%, #4a90e2 70%, #2b4fa8 100%);
        text-align: center;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
    }

    .hero h2 {
        font-size: 3rem;
        font-family: "Dosis";
        font-weight: bolder;
        letter-spacing: 2.5px;
    }

    .hero h5 {
        font-size: 1.25rem;
    }

    .games h3 {
        font-size: 2rem;
    }

    .games p {
        font-size: 1.2rem;
    }

    .games .card {
        transition: all 0.3s ease;
    }

    .games .card:hover {
        transform: scale(0.95);
    }
</style>
