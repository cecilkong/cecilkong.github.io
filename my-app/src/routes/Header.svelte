<script>
	import { page } from '$app/stores';
	import logo from '$lib/images/svelte-logo.svg';
	import github from '$lib/images/github.svg';
	import star_dark from '$lib/images/nav/star-dark.png'
	import star_light from '$lib/images/nav/star-light.png'
	import Button from './components/Button.svelte'
</script>

<header>
	<!-- <div class="corner">
		<a href="https://kit.svelte.dev">
			<img src={logo} alt="SvelteKit" />
		</a>
	</div> -->

	<nav>
		<!-- <svg viewBox="0 0 2 3" aria-hidden="true">
			<path d="M0,0 L1,2 C1.5,3 1.5,3 2,3 L2,0 Z" />
		</svg> -->
		<div class="title">
			<ul>
				<li class="no-padding">
					<a href="/home" class="cecil">Cecil Kong</a>
				</li>
			</ul>
		</div>
		<div class="page-links">
			<ul>
				<!-- <li aria-current={$page.url.pathname === '/' ? 'page' : undefined}>
					<a href="/">Home</a>
				</li>
				<li aria-current={$page.url.pathname === '/about' ? 'page' : undefined}>
					<a href="/about">About</a>
				</li>
				<li aria-current={$page.url.pathname.startsWith('/sverdle') ? 'page' : undefined}>
					<a href="/sverdle">Sverdle</a>
				</li> -->

				<!-- <li aria-current={$page.url.pathname === '/home' ? 'page' : undefined}> -->
				<li>
					<a href="/home">projects</a>
				</li>
				<!-- <li aria-current={$page.url.pathname === '/2D' ? 'page' : undefined}> -->
				<li>
					<a href="/2D">2D</a>
				</li>
				<!-- <li> aria-current={$page.url.pathname === '/3D' ? 'page' : undefined}> -->
				<li>
					<a href="/3D">3D</a>
				</li>
				<!-- <li aria-current={$page.url.pathname === '/my-about' ? 'page' : undefined}> -->
				<li>
					<a href="/my-about">About</a>
				</li>
				<li class="no-padding">
					<Button>
						<img src={star_dark} class="color-mode dark-icon" alt="Light/Dark Mode Toggle Icon" />
						<img src={star_light} class="color-mode light-icon" alt="Light/Dark Mode Toggle Icon" />
					</Button>
				</li>
			</ul>
		</div>
	</nav>

	<!-- <div class="corner">
		<a href="https://github.com/sveltejs/kit">
			<img src={github} alt="GitHub" />
		</a>
	</div> -->
</header>

<style>
	header {
		display: flex;
		/* justify-content: space-between; */
		justify-content: center;
		max-width: 64rem;
		/* border-style: dashed; */
		align-self: center;
		min-width: 64rem;
		max-width: 64rem;
		
	}

	.title {
		align-self: flex-start;
		/* border-style: solid; */
	}

	/* .page-links {
		align-self: flex-end;
		border-style: solid;
	} */

	.color-mode {
		width: 1.5em;
	}
	/* .corner {
		width: 3em;
		height: 3em;
	}

	.corner a {
		display: flex;
		align-items: center;
		justify-content: center;
		width: 100%;
		height: 100%;
	}

	.corner img {
		width: 2em;
		height: 2em;
		object-fit: contain;
	} */

	nav {
		display: flex;
		justify-content: space-between;
		--background: rgba(255, 255, 255, 0.7);
		font-family: var(--font-mono);
		/* border-style: dotted; */
		flex: auto;
		margin: 6vh 0vw 0vh 0vw;
	}

	/* svg {
		width: 2em;
		height: 3em;
		display: block;
		border-style: dotted;
	} */

	path {
		/* border-style: dotted; */
		fill: var(--background);
	}

	ul {
		/* border-style: dotted; */
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: space-between;
		align-items: center;
		list-style: none;
		background-size: contain;
		flex: auto;
	}

	.page-links {
		/* border-style: solid; */
		/* margin-left: 50px; */
	}

	li {
		/* border-style: dotted; */
		position: relative;
		height: 100%;
		/* border-style: dotted; */
		padding-right: 2.5vw;
	}

	.no-padding {
		padding: 0;
		font-weight: 100;
	}

	.cecil {
		font-style: normal;
		font-weight: 100;
		font-size: 1.2rem;
	}

	li[aria-current='page']::before {
		--size: 6px;
		content: '';
		width: 0;
		height: 0;
		position: absolute;
		top: 0;
		left: calc(50% - var(--size));
		border: var(--size) solid transparent;
		border-top: var(--size) solid var(--color-theme-1);
	}

	nav a {
		/* border-style: dotted; */
		display: flex;
		height: 100%;
		align-items: center;
		/* padding: 0 0.5rem; */
		color: var(--color-text);
		font-weight: 500;
		font-size: 1rem;
		text-transform: lowercase;
		letter-spacing: 0.05em;
		text-decoration: none;
		transition: color 0.2s linear;
	}

	a:hover {
		color: var(--color-theme-1);
	}

	:global(body) nav a {
		background-color: #F1F1F1;
		color: #131316;
		transition: background-color 0.3s;
	}

	:global(body.dark-mode) nav a {
		background-color: #131316;
		color: #F1F1F1;
		transition: background-color 0.3s;
	}

	.light-icon {
		display: none;
	}
	.dark-icon {
		display: inline;
	}

	:global(body.dark-mode) .light-icon {
		display: inline;
	}
	:global(body.dark-mode) .dark-icon {
		display: none;
	}
</style>
