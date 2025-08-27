<script>
	import ProjectListing from "$lib/components/ProjectListing.svelte";
</script>

<title>Projects - SRN's Site</title>

<main>
    <h1 class="mt-4">Projects</h1>
    <h5 class="mb-4">Projects I've worked on.</h5>
    
    <div class="d-flex flex-column gap-4 mb-4">
        <ProjectListing name="SRN Feud" description="<a href='https://chromewebstore.google.com/detail/srn-feud/koonghjejgkkfjbhplbkbbknhnhlogki' target='_none'>View on the Chrome Web Store</a> <br><br> A browser extension that connects to a TikTok Live chat and allows the viewers to compete against each other in Google Feud." image="/project_images/srn_feud.png" />
        <ProjectListing name="Crackix" description="An in-development studying app to make learning more engaging and fun. No public screenshots yet..." />
        <ProjectListing name="SAC" description="A private userscript designed to automatically host and protect Blooket games. Used on streams by Zander, Crazy Chicken Live, and a few others." />
        <ProjectListing name="Gimhoster" description="A private userscript designed to automatically host Gimkit games. Supports 1d, 2d, and creative gamemodes. Used by Crazy Chicken Live." />
        <ProjectListing name="BetterBanto" description="An extension to enhance functionality for banto.tv. Adds dark mode, trading features, solo mode, and many other neat features." />
        <ProjectListing name="SRN Voting" description="A simple script written in TypeScript that listens to a YouTube live chat and lets viewers vote for the next gamemode in either Blooket or Gimkit. Email me if you would like to use it." />
        <ProjectListing name="Pigbot" description="A discord bot written in TypeScript that has fun features, such as an 8-ball style guess feature, pick an option, a chatbot that uses machine learning, and other fun things." />
    </div>

    <p class="mb-4">... and more that I haven't listed yet.</p>
</main>

<style>
    h1 {
        font-family: "Patrick Hand";
        font-weight: 600;
        letter-spacing: 4px;
    }

    :root {
        background-color: #111111;
        overflow-x: hidden;
    }

    main {
        display: flex;
        flex-direction: column;
        align-items: center;
        height: 100vh;
        width: 100vw;
        background-color: #111111;
        color: white;
    }
</style>
