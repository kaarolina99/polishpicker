<script>
    import Navbar from "../Navbar.svelte";
    import PolishPickerComponent from "../PolishPickerComponent.svelte";
    import PolishList from "./PolishList.svelte";

    const polishes = [
    {name: "Red berries",
    color: "red",
    imageUrl: "https://www.holotaco.com/cdn/shop/files/HT-F_I-_0000s_0003_Layer9.jpg?v=1686779179&width=990",
    },
    {name: "Nightshade",
    color: "purple",
    imageUrl: "https://www.holotaco.com/cdn/shop/files/HT-DTE-_0000s_0004_Layer3.jpg?v=1691592919&width=990",
    },
    {name: "Nightshade2",
    color: "purple",
    imageUrl: "https://www.holotaco.com/cdn/shop/files/HT-DTE-_0000s_0002_Layer5.jpg?v=1691592909&width=990",
    },
    {name: "Nightshade3",
    color: "purple",
    imageUrl: "https://www.holotaco.com/cdn/shop/files/HT-DTE-_0000s_0004_Layer3.jpg?v=1691592919&width=990",
    },
    {name: "Nightshade4",
    color: "purple",
    imageUrl: "https://www.holotaco.com/cdn/shop/files/HT-DTE-_0000s_0004_Layer3.jpg?v=1691592919&width=990",
    },
    
]

</script>
<Navbar></Navbar>
Hello

<PolishList polishes = {polishes}></PolishList>

<style>



</style>