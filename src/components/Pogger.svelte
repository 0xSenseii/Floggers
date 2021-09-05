<script>
    const prices = {
        Zero: "0.34",
        Bee: "0.0.0799",
        Cat: "0.049",
        Dog: "0.0488",
        Elephant: "0.063",
        Frog: "0.049",
        Gorilla: "0.069",
        Llama: "0.0649",
        Mouse: "0.0643",
        Owl: "0.0489",
        Penguin: "0.049",
        RedPanda: "0.05",
        Turtle: "0.07",
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
