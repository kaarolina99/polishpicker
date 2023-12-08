<script>
    import ArtPickerComponent from "./ArtPickerComponent.svelte";
    import Navbar from "./Navbar.svelte";
    import PolishPickerComponent from "./PolishPickerComponent.svelte";

    
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

const arts = [
    {name: "Swirl",
    imageUrl: "https://www.instyle.com/thmb/Oc6bb8eRTNjpU-pquEYVabXYEP8=/750x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/PistsachioSwirl-ef5b87a0ca16471498020710a1cbd79c.jpg",
    },
    {name: "French",
    imageUrl: "https://www.instyle.com/thmb/ciF9zxUNWy96DtVcJ1OC7H9SbOs=/750x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/FrenchTips-bda8888f243b442c86cd966c4b769db5.jpg",
    },
    {name: "French2",
    imageUrl: "https://www.instyle.com/thmb/ciF9zxUNWy96DtVcJ1OC7H9SbOs=/750x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/FrenchTips-bda8888f243b442c86cd966c4b769db5.jpg",
    },
    {name: "French3",
    imageUrl: "https://www.instyle.com/thmb/ciF9zxUNWy96DtVcJ1OC7H9SbOs=/750x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/FrenchTips-bda8888f243b442c86cd966c4b769db5.jpg",
    },
    {name: "French4",
    imageUrl: "https://www.instyle.com/thmb/ciF9zxUNWy96DtVcJ1OC7H9SbOs=/750x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/FrenchTips-bda8888f243b442c86cd966c4b769db5.jpg",
    },
    
]

let variable = "hellooooo"

</script>

<Navbar></Navbar>
<ArtPickerComponent arts={arts}></ArtPickerComponent>
<PolishPickerComponent polishes={polishes}></PolishPickerComponent>

<style>
    @font-face {
    font-family: AdLib;
    src: url("/fonts/AdLibRegular copy/AdLib_Regular.ttf");
    font-weight: bold;
}




</style>