<script>
    const prices = {
        Zero: "0.35",
        Bee: "0.08",
        Cat: "0.077",
        Dog: "0.058",
        Elephant: "0.029",
        Frog: "0.029",
        Gorilla: "0.079",
        Llama: "0.0499",
        Mouse: "0.04",
        Owl: "0.04",
        Penguin: "0.04",
        RedPanda: "0.029",
        Turtle: "0.029",
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
