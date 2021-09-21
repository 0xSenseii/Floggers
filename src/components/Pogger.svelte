<script>
    const prices = {
        Zero: "0.35",
        Bee: "0.089",
        Cat: "0.059",
        Dog: "0.052",
        Elephant: "0.053",
        Frog: "0.068",
        Gorilla: "0.09",
        Llama: "0.08",
        Mouse: "0.065",
        Owl: "0.069",
        Penguin: "0.049",
        RedPanda: "0.051",
        Turtle: "0.09",
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
