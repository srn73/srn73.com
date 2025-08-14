<title>Home - SRN's Site</title>

<main>
    <h1>SRN's Site</h1>
    <h3>🛠️ Under Construction 🚧</h3>
</main>

<style>
    @keyframes float {
        0% {
            transform: translateX(-30vw) translateY(150px) rotateX(-180deg) scale(0);
            opacity: 40%;
        }
        100% {
            transform: translateX(0vw) translateY(0px) rotateX(360deg) scale(1);
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

    main * {
        animation: float 1s ease;
    }
</style>
