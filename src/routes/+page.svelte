<script>
    import ArtPickerComponent from "./ArtPickerComponent.svelte";
    import Navbar from "./Navbar.svelte";
    import PolishPickerComponent from "./PolishPickerComponent.svelte";


    
    const polishes = [
    {name: "Hot Take",
    color: "red",
    imageUrl: "https://www.holotaco.com/cdn/shop/files/HT-F_I-_0000s_0003_Layer9.jpg?v=1686779179&width=990",
    info: "Are your nails on fire, or are you just happy to see us? Paint on a Hot Take for a searing hot orange-red mani that makes a statement. Nobody can argue with the full coverage of this crème. Bright orange-leaning red polish with a crème formula. Full coverage in 2 coats.",
    },
    {name: "Nightshade",
    color: "purple",
    imageUrl: "https://www.holotaco.com/cdn/shop/files/HT-DTE-_0000s_0004_Layer3.jpg?v=1691592919&width=990",
    info: "Fall into some mani mischief by picking up a Nightshade. Get a dangerously delectable look in two to three coats of this rich eggplant purple polish. You can’t eat the polish, but you sure can slay with it. Aubergine-eggplant purple polish with a crème formula. Full coverage in 2-3 coats.",
    },
    {name: "Pinky Swear",
    color: "pink",
    imageUrl: "https://www.holotaco.com/cdn/shop/products/HT-Bottle-PinkySwear-2.jpg?v=1678502051&width=990",
    info: "Set your heart on a pink so cozy and coveted we know you’re Lowkey Blushing. Apply two to three coats of this rich, warm blush crème to satisfy your pink mani cravings. With coverage so obvious, we think it likes you back. Warm blush pink polish with a crème formula. Full coverage in 2-3 coats.",
    },
    {name: "Cold Slate",
    color: "blue",
    imageUrl: "https://www.holotaco.com/cdn/shop/files/HT-F_I-_0000s_0006_Layer12.jpg?v=1686780109&width=990",
    info: "Time to chill out and start over with a Cold Slate. In two coats, this steel-blue grey crème polish will have you living your best unbothered life. Hit the reset button with this clean, cool shade. Muted slate blue-grey polish with a crème formula. Full coverage in 2 coats.",
    },
    {name: "Crime and Punishmint",
    color: "green",
    imageUrl: "https://www.holotaco.com/cdn/shop/products/HT-Bottle-CrimeAndPunishmint-2.jpg?v=1678502047",
    info: "Guilty of committing nail offences? Your Crime and Punishmint is to hereby apply this perfect pastel mint polish to your fingertips. Failure to do so may result in further boring manicures. Vibrant pastel light mint green polish with a crème formula. Full coverage in 2 to 3 coats.",
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



</script>
<div class= "body">
<Navbar></Navbar>
<ArtPickerComponent arts={arts}></ArtPickerComponent>
<PolishPickerComponent polishes={polishes}></PolishPickerComponent>
<PolishPickerComponent polishes={polishes}></PolishPickerComponent>
</div>

<style>
    @font-face {
    font-family: AdLib;
    src: url("/fonts/AdLibRegular copy/AdLib_Regular.ttf");
    font-weight: bold;
}

.body{
    background-image: url(https://t3.ftcdn.net/jpg/02/97/02/48/360_F_297024828_Mxc3gHxDM1R8HpFWO5BH1NylqizJL1uY.jpg);
}

</style>