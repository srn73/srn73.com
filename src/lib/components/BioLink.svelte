<script lang="ts">
    export let name = "name";
    export let icon = "icon";
    export let href = "href";
    export let theme = "white";
</script>

<a class="biolink" href="{href}" target="_none">
    <img src="{icon}" alt="{name}" class="{theme}">
</a>

<style>
    .biolink {
        font-size: 20px;
        border-radius: 15px;
    }

    .biolink img {
        width: 50px;
        transition: transform 0.2s ease, filter 0.2s ease;
        transform: scale(1);
    }

    .biolink img:hover {
        transform: scale(0.85);
        filter: invert(1) brightness(80%);
    }

    .white {
        filter: invert(1) brightness(100%);
    }
</style>
