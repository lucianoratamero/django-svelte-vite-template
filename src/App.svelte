<script>
	import Counter from './lib/Counter.svelte';
	import Routes from './Routes.svelte';
</script>

<main>
	<h1>Hello world!</h1>

	<Counter />

	<h2>
		Here are some examples of code-splitted routes using <a href="https://github.com/AlexxNB/tinro"
			>tinro</a
		> (it's awesome!):
	</h2>
	<nav>
		<a href="/">Route 1</a>
		<a href="/route2">Route 2</a>
		<a href="/route3">Route 3</a>
	</nav>
	<Routes />

	<p>
		Visit <a href="https://svelte.dev">svelte.dev</a> to learn how to build Svelte apps.
	</p>

	<p>
		Check out <a href="https://github.com/sveltejs/kit#readme">SvelteKit</a> for the officially supported
		framework, also powered by Vite!
	</p>
</main>

<style>
	:root {
		font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell,
			'Open Sans', 'Helvetica Neue', sans-serif;
	}

	main {
		text-align: center;
		padding: 1em;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4rem;
		font-weight: 100;
		line-height: 1.1;
		margin: 2rem auto;
		max-width: 14rem;
	}

	p {
		max-width: 14rem;
		margin: 1rem auto;
		line-height: 1.35;
	}

	@media (min-width: 480px) {
		h1 {
			max-width: none;
		}

		p {
			max-width: none;
		}
	}
</style>
