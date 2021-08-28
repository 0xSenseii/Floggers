<script>
    const prices = {
        Zero: "0.5",
        Bee: "0.11",
        Cat: "0.099",
        Dog: "0.095",
        Elephant: "0.0889",
        Frog: "0.089",
        Llama: "0.1",
        Mouse: "0.07",
        Owl: "0.0888",
        RedPanda: "0.088",
        Penguin: "0.1",
        Gorilla: "0.1",
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
