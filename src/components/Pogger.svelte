<script>
    const prices = {
        Zero: "0.69",
        Bee: "0.0.089",
        Cat: "0.0945",
        Dog: "0.087",
        Elephant: "0.088",
        Frog: "0.08",
        Gorilla: "0.098",
        Llama: "0.08",
        Mouse: "0.088",
        Owl: "0.075",
        Penguin: "0.099",
        RedPanda: "0.0989",
        Turtle: "0.087",
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
