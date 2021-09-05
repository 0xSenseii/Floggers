<script>
    const prices = {
        Artemis: "15",
        AlienCat: "25",
        BubblegumGorilla: "2,5057",
        DiamondOwl: "420,69",
        DriftwoodTurtle: "4,999",
        FlamingRedPanda: "6",
        GoldenFrog: "10",
        IcePenguin: "300",
        Jellophant: "18",
        MarbleMouse: "4,205",
        RainbowLlama: "20",
        SilverBee: "14,99",
        ZombieDog: "5555,5",
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
