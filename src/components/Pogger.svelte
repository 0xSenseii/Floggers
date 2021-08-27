<script>
    const prices = {
        Zero: "0.495",
        Bee: "0.11",
        Cat: "0.09",
        Dog: "0.095",
        Elephant: "0.09",
        Frog: "0.089",
        Llama: "0.99",
        Mouse: "0.09",
        Owl: "0.099",
        RedPanda: "0.09",
        Penguin: "0.1",
        Gorilla: "0.1",
        Turtle: "0.09",
    };

    export let poggername;
    let price = prices[poggername];
</script>

<div class="cards__item">
    <a
        href="https://opensea.io/collection/spacepoggers?search[sortAscending]=true&search[sortBy]=PRICE&search[stringTraits][0][name]=Tribe&search[stringTraits][0][values][0]={poggername}"
    >
        <img
            src="imgs/{poggername}.png"
            alt={poggername}
            width="130"
            height="130"
        /></a
    >

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
