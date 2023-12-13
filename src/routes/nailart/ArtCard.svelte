<script>
    export let artName
    export let artImage
    export let artInfo
    console.log("hallo")


</script>

    
<div class="art-container">
    <img alt="art" src={artImage} style="width: 280px; height: 280px;">
    <div class="info-container">
        <p>Name: {artName}</p>
        <p>{artInfo}</p>
    </div>
</div>
    
<style>   
    
    .art-container {
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