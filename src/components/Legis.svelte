<script>
    const prices = {
        AlienCat: "10",
        BubblegumGorilla: "10",
        DiamondOwl: "420.69",
        DriftwoodTurtle: "19.999",
        FlamingRedPanda: "6.9",
        GoldenFrog: "15",
        IcePenguin: "4.2069",
        Jellophant: "18",
        MarbleMouse: "5.55",
        RainbowLlama: "20",
        SilverBee: "14.99",
        ZombieDog: "5",
    };

    export let legiName;
    let price = prices[legiName];
</script>

<div class="cards__item">
    <img src="imgs/{legiName}.png" alt={legiName} width="130" height="130" />
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
