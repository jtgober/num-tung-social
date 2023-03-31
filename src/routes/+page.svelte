<script>
  import Header from "../Header.svelte"
  import Carousel from "../Carousel.svelte";
  let image_collections = [
	"image1.png",
	"image2.png",
	"image3.png",	
	"image4.png",
    "image5.png"
];
</script>

<Header />

<h1>Welcome to SvelteKit</h1>
<p>
  <Carousel images={image_collections}/>
</p>
