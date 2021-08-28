<script>
	import Pogger from "./components/Pogger.svelte";
	import Head from "./components/Head.svelte";
	import Legis from "./components/Legis.svelte";
	import Wallet from "./components/Wallet.svelte";
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
	$: legistab = false;
	function showLegis() {
		legistab = true;
	}
	function showNormies() {
		legistab = false;
	}
	console.log(legistab);
</script>

<Head />

<main>
	<h1>Pogger Floor Prices</h1>
	<div class="cards">
		{#if !legistab}
			{#each pogs as pog}
				<Pogger poggername={pog.name} />
			{/each}
		{:else}
			{#each legis as pog}
				<Legis legiName={pog.name} />
			{/each}
		{/if}
	</div>

	<!-- <Category legis={legistab} /> -->

	<div class="category">
		<a class="legis" href="#" on:click|preventDefault={() => showLegis()}
			>Show Legis</a
		>
		<a
			class="normies"
			href="#"
			on:click|preventDefault={() => showNormies()}>Show Normies</a
		>
	</div>

	<Wallet />

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
		margin-top: 50px;
	}
	a {
		text-decoration: underline;
		color: beige;
	}
	a:hover {
		color: #ffcf22;
	}
	.legis {
		margin-right: 50px;
	}
	.normies {
		margin-left: 50px;
	}

	@media (max-width: 640px) {
		main {
			max-width: none;
		}
		.github-fork-ribbon {
			opacity: 0%;
		}
		.category {
			display: flex;
			align-items: center;
			justify-content: center;
		}
	}
</style>
