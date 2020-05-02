<script>
	import Card from './components/Card.svelte'
</script>

<main>
	<h1>RandomShow!</h1>
	<p>Estos son los últimos juegos que puedes descargar</p>
	<p>
		Powered by <a href="https://crackwatch.com/">CrackWatch</a>
	</p>

	<Card
		name="Resident Evil 3 Remake"
		description="El Juego aún no ha sido crackeado 💔"
		image="https://i1.wp.com/culturageek.com.ar/wp-content/uploads/2020/03/Culturageek.com_.ar-Resident-Evil-3-Review-1.jpg"
		urlBuy="https://store.steampowered.com/app/952060/RESIDENT_EVIL_3/?l=latam&curator_clanid=28542422"
		urlDownload=""
	/>
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