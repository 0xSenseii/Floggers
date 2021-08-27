<script>
	import Pogger from "./components/Pogger.svelte";
	let pogs = [
		{
			name: "Zero",
		},
		{
			name: "Bee",
		},
		{
			name: "Cat",
		},
		{
			name: "Dog",
		},
		{
			name: "Elephant",
		},

		{
			name: "Llama",
		},
		{
			name: "Mouse",
		},
		{
			name: "Owl",
		},
		{
			name: "RedPanda",
		},
		{
			name: "Penguin",
		},
		{
			name: "Gorilla",
		},
		{
			name: "Turtle",
		},
		{
			name: "Frog",
		},
	];
</script>

<svelte:head>
	<meta charset="UTF-8" />
	<meta http-equiv="X-UA-Compatible" content="IE=edge" />
	<meta name="viewport" content="width=device-width, initial-scale=1.0" />
	<link
		rel="icon"
		href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>💰</text></svg>"
	/>
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
	<link
		href="https://fonts.googleapis.com/css2?family=Press+Start+2P&display=swap"
		rel="stylesheet"
	/>
	<title>Poggers Floor Prices</title>
</svelte:head>

<main>
	<h1>Pogger Floor Prices</h1>
	<div class="cards">
		{#each pogs as pog}
			<Pogger poggername={pog.name} />
		{/each}
	</div>
</main>

<style>
	:global(body) {
		font-family: "Press Start 2P", cursive;
		text-align: center;
		font-size: 12px;
		color: beige;
		background: #111;
	}

	h1 {
		margin-top: 75px;
		margin-bottom: 100px;
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
