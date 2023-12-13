<script>
    import Navbar from "../Navbar.svelte";
    import ArtList from "./ArtList.svelte";


    const arts = [
    {name: "Swirl",
    imageUrl: "https://www.instyle.com/thmb/Oc6bb8eRTNjpU-pquEYVabXYEP8=/750x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/PistsachioSwirl-ef5b87a0ca16471498020710a1cbd79c.jpg",
    info: "Swirl nail art is a creative and stylish nail design that involves incorporating swirling patterns into your nail polish or nail enhancements. It's a versatile and eye-catching design that can be customized in various ways to suit your personal style.",
    },
    {name: "French",
    imageUrl: "https://www.instyle.com/thmb/ciF9zxUNWy96DtVcJ1OC7H9SbOs=/750x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/FrenchTips-bda8888f243b442c86cd966c4b769db5.jpg",
    info: "French nail art is a classic and timeless manicure style that is known for its clean and elegant appearance. French nail art, in its various forms, remains a popular choice for those seeking a sophisticated and refined manicure. Its adaptability to different styles and occasions makes it a classic option that continues to be reinvented with modern trends."
    },
    {name: "Aura",
    imageUrl: "https://www.byrdie.com/thmb/EWXQJc1p1yZlzV2FliRqp8KNQ6I=/750x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/PalePinkAuraNails-1fe51f6406b64de097cc6b944631ad8d.jpg",
    info: "Aura nail art is a mesmerizing and ethereal manicure style that often involves creating a soft and dreamy look reminiscent of an aura or glow. It's perfect for those who appreciate subtle and otherworldly aesthetics in their manicure.",
    },
    {name: "Half Moons",
    imageUrl: "https://www.instyle.com/thmb/HR5JfBmekp8ce67LutBGFacCB9M=/1500x0/filters:no_upscale():max_bytes(150000):strip_icc():format(webp)/MonocromaticHalfMoons-0dbc358d55d5407f944030de7f0c8614.jpg",
    info: "Half-moon nail art is a classic and versatile manicure style that features a crescent or half-moon shape near the cuticle area of the nail. This style allows for creativity and personalization, making it a popular choice for both casual and formal occasions.",
    },
    {name: "Marble",
    imageUrl: "https://cdn.cliqueinc.com/posts/302334/marble-nail-designs-302334-1662764586281-main.900x0c.jpg?interlace=true&quality=70",
    info: "Marble nail art is a stylish and sophisticated manicure technique that replicates the appearance of natural marble stone on the nails. t's a favorite among those who appreciate sophisticated and intricate manicure styles."
    },
    
]

</script>
<Navbar></Navbar>

<div class="body">
<ArtList arts={arts}></ArtList>     
</div>

<style>
.body{
    background-image: url(https://t3.ftcdn.net/jpg/02/97/02/48/360_F_297024828_Mxc3gHxDM1R8HpFWO5BH1NylqizJL1uY.jpg);
}


</style>
