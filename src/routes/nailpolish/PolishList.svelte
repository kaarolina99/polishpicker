<script>
    import PolishCard from "./PolishCard.svelte";

    export let polishes


console.log("hello", polishes[0].imageUrl)

</script>

<div class="container">  
    <div class="gridcols">
        {#each polishes as polish}
            <PolishCard polishName={polish.name} polishImage={polish.imageUrl} polishColor={polish.color} polishInfo={polish.info}></PolishCard>
        {/each}
    </div>
</div>


<style>
    .container {
        width: 100vw;
        gap: 10px;
        padding-top: 50px;
    }
    .gridcols {
        display: grid;
        grid-column: 1;
        grid-template-columns: repeat(2, minmax(0, 1fr));
        gap: 100px;
        justify-content: center;
    }



</style>


