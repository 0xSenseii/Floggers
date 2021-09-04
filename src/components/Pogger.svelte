<script>
    const prices = {
        Zero: "0.48",
        Bee: "0.0.08",
        Cat: "0.05",
        Dog: "0.0649",
        Elephant: "0.055",
        Frog: "0.0648",
        Gorilla: "0.057",
        Llama: "0.0649",
        Mouse: "0.069",
        Owl: "0.049",
        Penguin: "0.07",
        RedPanda: "0.065",
        Turtle: "0.0474",
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
