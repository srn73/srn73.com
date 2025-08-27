<script lang="ts">
    export let name = "Project";
    export let description = "Lorem ipsum dolor sit amet, consectetur adipiscing elit.";
    export let image = "";
</script>

<div class="project-card text-center">
    {#if image}
        <div class="d-flex flex-column mb-2 fw-bold">
            <img src="{image}" class="mb-2" alt="Project example">
            <a href="{image}" target="_none">View full image</a>
        </div>
    {/if}
    <h3>{name}</h3>
    <p>{@html description}</p>
</div>

<style>
    .project-card {
        width: 100%;
        background-color: rgb(73, 73, 73);
        border: 3px solid #B0B0B0;
        border-radius: 15px;
        padding: 1rem;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    .project-card p {
        margin: 0;
        max-width: 40vw;
    }

    .project-card img {
        width: 40vw;
        height: auto;
        border-radius: 15px;
    }
</style>
