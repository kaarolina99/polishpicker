<script>
    export let polishes

    
    let currentPolishIndex = 0;
    let currentImageIndex = 0;

    function nesteNederst(){
        console.log("nesteN", currentPolishIndex, currentImageIndex)
        currentPolishIndex++;
        currentImageIndex++;

        if ( currentPolishIndex >= polishes.length) {
            currentPolishIndex = 0;
        }
        if (currentImageIndex >= polishes.length) {
            currentImageIndex = 0;
        }

}
    
function tilbakeNederst(){
    console.log("tilbakeN", currentPolishIndex, currentImageIndex)

    if ( currentPolishIndex <= 0) {
        currentPolishIndex = polishes.length;
    }

    if (currentImageIndex <= 0) {
        currentImageIndex = polishes.length;
    }

    currentPolishIndex=currentPolishIndex-1;
    currentImageIndex=currentImageIndex-1;

}
</script>



<div class="container">        
    <div class="polish1" style="position: relative;">
        <img id="color1" alt="color1" src={polishes[currentImageIndex].imageUrl} style="width: 280px; height: 280px;">
        <p class="overlay-text1">{polishes[currentPolishIndex].name}</p>
        <p class="overlay-text">{polishes[currentPolishIndex].color}</p>
    </div>
</div>


<div class="polish1_container">
    <div>
        <button class ="button button4" id="tilbakeN" on:click={tilbakeNederst}> TILBAKE </button>
        <button class ="button button5" id="stoppN" > STOPP </button>
        <button class ="button button6" id="nesteN" on:click={nesteNederst}> NESTE </button>
    </div>
</div>



<style>
.container {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center; 
    }
    
    .overlay-text1{
        font-weight: 550;
        text-align: center;
        position: absolute;
        top: 5px; 
        left: 50%; 
        transform: translate(-50%); 
        color: white;
    }
    .overlay-text{
        font-weight: 550;
        text-align: center;
        position: absolute;
        bottom: -10px; 
        left: 50%; 
        transform: translateX(-50%); 
        color: white;
    }
    
    .polish1{
        width: 280px;
        height: 280px;
        border: 2px solid blue;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    
    .polish1_container{
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

