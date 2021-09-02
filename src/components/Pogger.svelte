<script>
    const prices = {
        Zero: "0.55",
        Bee: "0.0.087",
        Cat: "0.089",
        Dog: "0.08",
        Elephant: "0.07",
        Frog: "0.0789",
        Gorilla: "0.08",
        Llama: "0.08",
        Mouse: "0.075",
        Owl: "0.088",
        Penguin: "0.09",
        RedPanda: "0.078",
        Turtle: "0.078",
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
