<script>
    const prices = {
        Zero: "0.65",
        Bee: "0.11",
        Cat: "0.099",
        Dog: "0.095",
        Elephant: "0.09",
        Frog: "0.089",
        Llama: "0.099",
        Mouse: "0.09",
        Owl: "0.099",
        RedPanda: "0.09",
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
