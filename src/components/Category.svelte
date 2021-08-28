<script>
    export let legis;
    function showLegis() {
        legis = true;
        console.log("clicked");
    }
</script>

<div class="category">
    <a href="#" on:click|preventDefault={() => showLegis()}>Show Legis</a>
</div>

<style>
    .category {
        margin-top: 100px;
    }
    a {
        text-decoration: underline;
        color: beige;
    }
    a:hover {
        color: #ffcf22;
    }
</style>
