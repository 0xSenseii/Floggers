<script>
    const prices = {
        Zero: "0.65",
        Bee: "0.0.085",
        Cat: "0.079",
        Dog: "0.079",
        Elephant: "0.078",
        Frog: "0.079",
        Gorilla: "0.079",
        Llama: "0.079",
        Mouse: "0.079",
        Owl: "0.08",
        Penguin: "0.079",
        RedPanda: "0.078",
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
