<script>
    const prices = {
        Zero: "0.32",
        Bee: "0.098",
        Cat: "0.07",
        Dog: "0.055",
        Elephant: "0.045",
        Frog: "0.045",
        Gorilla: "0.075",
        Llama: "0.075",
        Mouse: "0.05",
        Owl: "0.08",
        Penguin: "0.049",
        RedPanda: "0.059",
        Turtle: "0.05",
    };

    export let poggername;
    let price = prices[poggername];
</script>

<div class="cards__item">
    <img
        src="imgs/{poggername}.png"
        alt={poggername}
        width="130"
        height="130"
    />

    <p>{price}Ξ</p>
</div>

<style>
    .cards__item {
        margin: 2px;
    }
    img {
        border-radius: 3%;
    }
</style>
