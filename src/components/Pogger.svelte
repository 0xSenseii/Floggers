<script>
    const prices = {
        Zero: "0.749",
        Bee: "0.1",
        Cat: "0.099",
        Dog: "0.0975",
        Elephant: "0.088",
        Frog: "0.088",
        Gorilla: "0.1",
        Llama: "0.1",
        Mouse: "0.088",
        Owl: "0.09",
        Penguin: "0.1",
        RedPanda: "0.089",
        Turtle: "0.092",
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
