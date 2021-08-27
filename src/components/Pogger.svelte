<script>
    const prices = {
        zero: "0.495",
        bzzz: "0.11",
        cato: "0.09",
        dogo: "0.09",
        eli: "0.1",
        frogo: "0.1",
        llamo: "0.1",
        mouse: "0.09",
        owlo: "0.1",
        pando: "0.1",
        pengu: "0.1",
        rilla: "0.1",
        turto: "0.09",
    };

    export let poggername;
    let price = prices[poggername];
</script>

<div class="cards__item">
    <img
        src="poggers/{poggername}.png"
        alt={poggername}
        width="130"
        height="130"
    />

    <p>{price} ETH</p>
</div>

<style>
    .cards__item {
        margin: 2px;
    }
    img {
        border-radius: 3%;
    }
</style>
