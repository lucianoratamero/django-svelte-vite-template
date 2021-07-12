<script>
	import { onMount } from 'svelte';

	import { Route } from 'tinro';
	let Route1, Route2, Route3;

	onMount(async () => {
		Route1 = (await import('./routes/Route1.svelte')).default;
		Route2 = (await import('./routes/Route2.svelte')).default;
		Route3 = (await import('./routes/Route3.svelte')).default;
	});
</script>

<Route path="/"><svelte:component this={Route1} /></Route>
<Route path="/route2"><svelte:component this={Route2} /></Route>
<Route path="/route3"><svelte:component this={Route3} /></Route>
