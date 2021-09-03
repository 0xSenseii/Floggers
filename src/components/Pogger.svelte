<script>
    const prices = {
        Zero: "0.53",
        Bee: "0.0.08",
        Cat: "0.065",
        Dog: "0.069",
        Elephant: "0.065",
        Frog: "0.068",
        Gorilla: "0.065",
        Llama: "0.065",
        Mouse: "0.065",
        Owl: "0.07",
        Penguin: "0.065",
        RedPanda: "0.065",
        Turtle: "0.0675",
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
