<script>
    const prices = {
        Zero: "0.79",
        Bee: "0.0.0989",
        Cat: "0.0835",
        Dog: "0.0975",
        Elephant: "0.08",
        Frog: "0.089",
        Gorilla: "0.098",
        Llama: "0.09",
        Mouse: "0.08",
        Owl: "0.08",
        Penguin: "0.079",
        RedPanda: "0.085",
        Turtle: "0.079",
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
