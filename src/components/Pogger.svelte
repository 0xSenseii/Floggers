<script>
    const prices = {
        Zero: "0.39",
        Bee: "0.069",
        Cat: "0.0489",
        Dog: "0.05",
        Elephant: "0.0399",
        Frog: "0.039",
        Gorilla: "0.055",
        Llama: "0.0384",
        Mouse: "0.045",
        Owl: "0.042",
        Penguin: "0.04",
        RedPanda: "0.06",
        Turtle: "0.05",
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
