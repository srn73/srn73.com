<script>
	import BioLink from "$lib/components/BioLink.svelte";

</script>
<title>Home - SRN's Site</title>

<main>
    <div class="profile-card">
        <img class="mb-3 rounded-pill" src="https://cdn.discordapp.com/avatars/546102590585438239/fb7d003d071f608c53aad7eb49dab350.webp" alt="My pfp">
        <h1 class="mb-3">SRN's Site</h1>
        <h5 class="mb-4">coding, content creation, and gaming</h5>
        
        <div class="d-flex gap-2 mb-4">
            <BioLink name="YouTube" icon="/icons/youtube.svg" href="https://youtube.com/@srns_stuff" theme="white" />
            <BioLink name="TikTok" icon="/icons/tiktok.svg" href="https://tiktok.com/@srns_stuff1" theme="white" />
            <BioLink name="Instagram" icon="/icons/instagram.svg" href="https://instagram.com/srns_stuff" theme="white" />
            <BioLink name="Discord" icon="/icons/discord.svg" href="https://discord.com/users/546102590585438239" theme="white" />
            <BioLink name="Twitter" icon="/icons/twitter.svg" href="https://x.com/@srns_stuff" theme="white" />
            <BioLink name="Email" icon="/icons/envelope.svg" href="mailto:contact@srn73.com" theme="white" />
        </div>

        <a class="fs-5 fw-bold text-white" href="/projects">Projects</a>
    </div>
</main>

<style>
    @keyframes float {
        0% {
            transform: scale(0);
            opacity: 0%;
        }
        100% {
            transform: scale(1);
            opacity: 100%;
        }
    }

    h1 {
        font-family: "Patrick Hand";
        font-weight: 600;
        letter-spacing: 4px;
    }

    main {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 100vh;
        background-color: #111111;
        color: white;
    }

    .profile-card {
        animation: float 1s ease;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        color: white;
        background: linear-gradient(90deg, #265bbd, #0e419d);
        padding: 2rem;
        border: 3px solid #6a9eff;
        border-radius: 20px;
    }
</style>
