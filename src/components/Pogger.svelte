<script>
    const prices = {
        Zero: "0.35",
        Bee: "0.08",
        Cat: "0.11",
        Dog: "0.0488",
        Elephant: "0.045",
        Frog: "0.0439",
        Gorilla: "0.08",
        Llama: "0.0439",
        Mouse: "0.045",
        Owl: "0.0553",
        Penguin: "0.075",
        RedPanda: "0.05",
        Turtle: "0.045",
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
