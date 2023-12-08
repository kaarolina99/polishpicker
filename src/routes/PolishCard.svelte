<script>
    export let polishName
    export let polishImage
    export let polishColor

    console.log(polishImage)
    
    let currentPolishIndex = 0;
    let currentImageIndex = 0;

    function nesteNederst(){
    currentPolishIndex++;
    currentImageIndex++;

    if ( currentPolishIndex >= polishes.length) {
        currentPolishIndex = 0;
    }
    if (currentImageIndex >= 3) {
        currentImageIndex = 0;
    }

}
    
function tilbakeNederst(){
    if ( currentPolishIndex <= 0) {
        currentPolishIndex = polishes.length;
    }

    if (currentImageIndex < 0) {
        currentImageIndex = 2;
    }

    currentPolishIndex=currentPolishIndex-1;
    currentImageIndex=currentImageIndex-1;

}



    </script>
    
    
    <div class="container">        
            <div class="polish1" style="position: relative;">
                <p> {polishName}</p>
                <img id="color1" alt="color1" src={polishImage} style="width: 280px; height: 280px;">
                <p> {polishColor}</p>
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
        height: 100vh; 
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
    