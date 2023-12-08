<script>
    import PolishCard from "./PolishCard.svelte";

    export let polishes


console.log("hello", polishes[0].imageUrl)

</script>

{#each polishes as polish}
    <PolishCard polishName={polish.name} polishImage={polish.imageUrl} polishColor={polish.color}></PolishCard>
{/each}





<style>


</style>
