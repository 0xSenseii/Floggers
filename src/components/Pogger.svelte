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
        AlienCat: "10",
        BubblegumGorilla: "10",
        DiamondOwl: "420.69",
        DriftwoodTurtle: "19.999",
        FlamingRedPanda: "7.5",
        GoldenFrog: "15",
        IcePenguin: "4.2069",
        Jellophant: "18",
        MarbleMouse: "5.55",
        RainbowLlama: "20",
        SilverBee: "14.99",
        ZombieDog: "5555.55",
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
        /* background: #ffcf22;
        border-radius: 3%; */
    }
    img {
        border-radius: 3%;
    }
</style>
