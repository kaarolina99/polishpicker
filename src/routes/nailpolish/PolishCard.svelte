<script>
    export let polishName
    export let polishColor
    export let polishImage
    export let polishInfo
    
    // console.log(polish.Info[3])

</script>

    
<div class="polish-container">
    <img alt="color" src={polishImage} style="width: 280px; height: 280px;">
    <div class="info-container">
        <p>Name: {polishName}</p>
        <p>Color: {polishColor}</p>
        <p>{polishInfo}</p>
    </div>
</div>
    
<style>   
    
    .polish-container {
        border: 2px solid red;
        background-color: #04063A;
        display: flex;
        align-items: center;
        max-width: 550px;
        max-height: 550px;
    }

    .info-container {
        margin-top: 10px;
        margin-left: 15px;
        margin-right: 5px;
        color:  #dcc2ff;
    }

    </style>
    
    