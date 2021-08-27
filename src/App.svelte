<script>
	import Pogger from "./components/Pogger.svelte";
	let pogs = [
		{
			name: "zero",
		},
		{
			name: "bzzz",
		},
		{
			name: "cato",
		},
		{
			name: "dogo",
		},
		{
			name: "eli",
		},
		{
			name: "frogo",
		},
		{
			name: "llamo",
		},
		{
			name: "mouse",
		},
		{
			name: "owlo",
		},
		{
			name: "pando",
		},
		{
			name: "pengu",
		},
		{
			name: "rilla",
		},
		{
			name: "turto",
		},
	];
</script>

<svelte:head>
	<meta charset="UTF-8" />
	<meta http-equiv="X-UA-Compatible" content="IE=edge" />
	<meta name="viewport" content="width=device-width, initial-scale=1.0" />
	<title>Poggers Floor Prices</title>
</svelte:head>

<main>
	<h1>💰 Poggers Floor 💰</h1>
	<div class="cards">
		{#each pogs as pog}
			<Pogger poggername={pog.name} />
		{/each}
	</div>
</main>

<style>
	:global(body) {
		text-align: center;
		color: beige;
		background: #111;
	}

	h1 {
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 400;
		color: #ffcf22;
	}

	.cards {
		display: flex;
		align-items: center;
		justify-content: center;
		/* Put a card in the next row when previous cards take all width */
		flex-wrap: wrap;
		padding-left: 2em;
		padding-right: 2em;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
