<script>
    const prices = {
        Bee: "0.11",
        Cat: "0.09",
        Dog: "0.09",
        Elephant: "0.1",
        Frog: "0.1",
        Llama: "0.1",
        Mouse: "0.09",
        Owl: "0.1",
        RedPanda: "0.1",
        Penguin: "0.1",
        Gorilla: "0.1",
        Turtle: "0.09",
        Zero: "0.495",
    };

    export let poggername;
    let price = prices[poggername];
</script>

<div class="cards__item">
    <a
        href="https://opensea.io/collection/spacepoggers?search[sortAscending]=true&search[sortBy]=PRICE&search[stringTraits][0][name]=Tribe&search[stringTraits][0][values][0]={poggername}"
    >
        <img
            src="poggers/{poggername}.png"
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
