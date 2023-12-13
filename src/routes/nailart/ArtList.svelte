<script>
    import ArtCard from "./ArtCard.svelte";

    export let arts


console.log("hello", arts[0].imageUrl)

</script>

<div class="container">  
    <div class="gridcols">
        {#each arts as art}
            <ArtCard artName={art.name} artImage = {art.imageUrl} artInfo={art.info}></ArtCard>
        {/each}
    </div>
</div>
<!-- polishInfo={polish.info} -->

<style>
    .container {
        width: 100vw;
        gap: 15px;
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
