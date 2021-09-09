<script>
    const prices = {
        Zero: "0.28",
        Bee: "0.08",
        Cat: "0.045",
        Dog: "0.043",
        Elephant: "0.045",
        Frog: "0.043",
        Gorilla: "0.039",
        Llama: "0.04",
        Mouse: "0.045",
        Owl: "0.039",
        Penguin: "0.045",
        RedPanda: "0.043",
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
