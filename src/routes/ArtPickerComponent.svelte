<script>
    export let arts
    
    console.log(arts[3].imageUrl)


    let currentArtIndex = 0
    let currentImageIndex = 0;


    function nesteOverst(){
    console.log("nesteO", currentArtIndex, currentImageIndex)
    currentArtIndex++;
    currentImageIndex++;


    if ( currentArtIndex >= arts.length) {
        currentArtIndex = 0;
    }
    if (currentImageIndex >= 5) {
        currentImageIndex = 0;
    }

}

function tilbakeOverst(){
    console.log("tilbakeO", currentArtIndex, currentImageIndex)
    if ( currentArtIndex <= 0) {
        currentArtIndex = arts.length;
    }
    if (currentImageIndex <= 0) {
        currentImageIndex = 5;
    }
    currentArtIndex=currentArtIndex-1;
    currentImageIndex=currentImageIndex-1;

}

</script>



<div class="container">        
    <div class="nailart" style="position: relative;">
        <p> {arts[currentArtIndex].name}</p>
        <img id="color1" alt="color1" src={arts[currentImageIndex].imageUrl} style="width: 280px; height: 280px;">
    </div>
    
</div>

<div class="nailart_container">
    <div>
        <button class ="button button4" id="tilbakeN" on:click={tilbakeOverst}> TILBAKE </button>
        <button class ="button button5" id="stoppN" > STOPP </button>
        <button class ="button button6" id="nesteN" on:click={nesteOverst}> NESTE </button>
    </div>
</div>




<style>
.container {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center; 
        padding-top: 100px;
    }
    
    
    .nailart{
        width: 280px;
        height: 280px;
        border: 2px solid blue;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    
    .nailart_container{
        background-color: black;
        width: 420px;
        height: 70px;
        display: flex;
        justify-content: center;
        align-items: center;
        margin: auto;
    }
    
    
    .button{
        color: white;
        padding: 16px 32px;
        text-align: center;
        text-decoration: none;
        display: inline-block;
        font-size: 16px;
        font-family: AdLib;
        margin: 4px 2px;
        transition-duration: 0.4s;
        cursor: pointer;
    }
    
    .button4 {
        background-color: #666666; 
        color: black; 
        border: 3px solid #383838;
    }
    .button4:hover {
        background-color: #740AFF;
        color: white;
        border: 3px solid #04063A
    }
    .button5 {
        background-color: #666666; 
        color: black; 
        border: 3px solid #383838;
    }
    .button5:hover {
        background-color: #740AFF;
        color: white;
        border: 3px solid #04063A
    }
    .button6 {
        background-color: #666666; 
        color: black; 
        border: 3px solid #383838;
    }
    .button6:hover {
        background-color: #740AFF;
        color: white;
        border: 3px solid #04063A;
    }

</style>