<script>
	import GlobalStyles from './GlobalStyles.svelte';
	export let name;
</script>

<GlobalStyles />

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<style lang="scss">
	@import "../scss/variables.scss";
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
		background: $background-color;
	}

	h1 {
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 500;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>