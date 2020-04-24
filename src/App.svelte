<script>
	import Card from './components/Card.svelte'
	export let name;
	export let lastName;
	
	setTimeout(() => lastName = 'holus', 3000)
</script>

<main>
	<!-- <h1>Hello {name} {lastName}!</h1> -->
	<h1>RandomShow!</h1>
	<p>Estos son los últimos juegos que puedes descargar</p>
	<p>Powered by <a href="https://svelte.dev/tutorial">CrackWatch</a>.</p>

	<Card />
</main>

<style>
	/* variable globals */
	:global(:root) {
		--background-color: #292C4F;
		--background-color__card: #363868;

		--text-primary: #292C4F;
		--text-default: #FEFEFE;
		--text-info: #59D2E0;
		--text-danger: #ff3e00;
	}

	/* global styles */
	:global(body) {
		background-color: var(--background-color);
		color: var(--text-default);
	}

	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: var(--text-danger);
		text-transform: uppercase;
		font-size: 2em;
		font-weight: 200;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>