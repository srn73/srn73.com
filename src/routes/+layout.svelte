<script lang="ts">
	import favicon from '$lib/assets/favicon.svg';
	import 'bootstrap/dist/css/bootstrap.min.css';

	export const prerender = true;

	let { children } = $props();
</script>

<style>
	@font-face {
		font-family: 'Patrick Hand';
		src: url('/fonts/PatrickHand-Regular.ttf') format('truetype');
		font-weight: normal;
		font-style: normal;
	}

	@font-face {
		font-family: 'Poppins';
		src: url('/fonts/Poppins-Bold.ttf') format('truetype');
		font-weight: normal;
		font-style: normal;
	}
	
	@font-face {
		font-family: 'Dosis';
		src: url('/fonts/Dosis-VariableFont_wght.ttf') format('truetype');
		font-weight: normal;
		font-style: normal;
	}
</style>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>

<div data-bs-theme="dark">
	{@render children?.()}
</div>
