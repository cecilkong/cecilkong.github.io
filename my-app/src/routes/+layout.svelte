<script>
	import Header from './Header.svelte';
	import '../app.css';
	import { fade } from 'svelte/transition';
	import { page } from '$app/stores';
	import { linear, quadIn, quadOut } from 'svelte/easing';
</script>

<div class="app">
	<Header />
	<main>
			{#key $page.url.pathname}
				<div in:fade={{ duration: 800, easing: quadOut}}>
				<slot />
				</div>
			{/key}
	</main>
	<footer>
		<p>© cecil kong 2025</p>
	</footer>
	<div class="line"></div>
</div>

<style>
	.app {
		/* border-style: dotted; */
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	main {
		/* border-style: dotted; */
		flex: 1;
		display: flex;
		flex-direction: column;
		width: 100%;
		max-width: 64rem;
		margin: 0 auto;
		box-sizing: border-box;
		overflow-x: hidden;
	}

	footer {
		/* border-style: dotted; */
		display: flex;
		flex: 1;
		max-width: 64rem;
		box-sizing: border-box;
		width: 100%;
		flex-direction: column;
		padding: 10px;
		margin: 0 auto;
	}

	.line {
  		border-bottom: 1.2px solid #000000;
		margin-bottom: 4vh;
	}

	:global(body.dark-mode) .line {
  		border-bottom: 1.2px solid #ffffff;
		margin-bottom: 4vh;
	}

	@media (min-width: 480px) {
		footer {
			padding: 12px 0;
		}
	}
</style>
