<script lang="ts">
	import { page } from "$app/state";
	import { onMount } from "svelte";

    let pages = [
        { name: "Home", path: "/streamtools" },
    ];
</script>

<nav class="navbar navbar-expand-lg">
	<div class="container-fluid">
		<a class="navbar-brand" href="/streamtools">Stream Tools</a>
		<button
			class="navbar-toggler"
			type="button"
			data-bs-toggle="collapse"
			data-bs-target="#navbarSupportedContent"
			aria-controls="navbarSupportedContent"
			aria-expanded="false"
			aria-label="Toggle navigation"
		>
			<span class="navbar-toggler-icon"></span>
		</button>
		<div class="collapse navbar-collapse" id="navbarSupportedContent">
			<ul class="navbar-nav me-auto mb-2 mb-lg-0">
                {#each pages as pagee}
                    <li class="nav-item">
                        <a class="nav-link {pagee.path == `${page.route.id}` ? "active" : ""}" aria-current="page" href="{pagee.path}">{pagee.name}</a>
                    </li>
                {/each}
			</ul>
		</div>
	</div>
</nav>

<style>
    .navbar {
        background-color: #222222;
		position: sticky;
		top: 0;
    }
</style>
