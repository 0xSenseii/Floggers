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
	const legis = [
		{
			name: "AlienCat",
		},
		{
			name: "BubblegumGorilla",
		},
		{
			name: "DiamondOwl",
		},
		{
			name: "DriftwoodTurtle",
		},
		{
			name: "FlamingRedPanda",
		},
		{
			name: "GoldenFrog",
		},
		{
			name: "IcePenguin",
		},
		{
			name: "Jellophant",
		},
		{
			name: "MarbleMouse",
		},
		{
			name: "RainbowLlama",
		},
		{
			name: "SilverBee",
		},
		{
			name: "ZombieDog",
		},
	];
	let legistab = false;
	function showLegis() {
		legistab = true;
	}
	funciton;
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
	<link
		rel="stylesheet"
		href="https://cdnjs.cloudflare.com/ajax/libs/github-fork-ribbon-css/0.2.3/gh-fork-ribbon.min.css"
		integrity="sha512-TktJbycEG5Van9KvrSHFUcYOKBroD7QCYkEe73HAutODCw9QTFcvF6fuxioYM1h6THNudK1GjVidazj6EslK4A=="
		crossorigin="anonymous"
		referrerpolicy="no-referrer"
	/>
	<title>Poggers Floor Prices</title>
</svelte:head>

<main>
	<h1>Pogger Floor Prices</h1>
	<div class="cards">
		{#if !legistab}
			{#each pogs as pog}
				<Pogger poggername={pog.name} />
			{/each}
		{:else}
			{#each legis as pog}
				<Pogger poggername={pog.name} />
			{/each}
		{/if}
	</div>
	<div class="category">
		<div class="normies">Normies</div>
		<div class="legis" on:click={showLegis()}>Legis</div>
	</div>
	<a
		class="github-fork-ribbon left-bottom"
		href="https://twitter.com/0xSensei"
		target="_blank"
		data-ribbon="🐦 Twitter 🐦"
		title="Fork me on GitHub"
	/>
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

	.category {
		display: flex;
		align-items: center;
		justify-content: center;
	}
	.normies {
		padding-right: 50px;
	}
	.legis {
		padding-left: 50px;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
