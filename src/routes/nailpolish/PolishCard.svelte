<script>
    export let polishName
    export let polishImage
    export let polishColor
    // halo

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
    

    
    
    
    <style>
    
    </style>
    