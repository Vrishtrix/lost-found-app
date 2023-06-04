<script>
	import { LazyCSSProvider } from '@master/css.svelte';

	import '@master/normal.css/dist/index.css';

	const loadConfig = import('../master.css');
</script>

<svelte:head>
	<link
		href="https://fonts.googleapis.com/css?family=Montserrat"
		rel="stylesheet"
	/>

	<style>
		html,
		body {
			font-family: Montserrat;
		}
	</style>
</svelte:head>

<LazyCSSProvider config={loadConfig}>
	<slot />
</LazyCSSProvider>
