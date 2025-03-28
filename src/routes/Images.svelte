<script>
  // @ts-nocheck
  import Buttons from "./Buttons.svelte";

  import img1 from "$lib/images/20240727_153951.jpg";
  import img2 from "$lib/images/20240723_171818.jpg";
  import img3 from "$lib/images/20240804_190422.jpg";
  import img4 from "$lib/images/20240721_232639.jpg";
  import img5 from "$lib/images/20240812_143245.jpg";
  import img6 from "$lib/images/20240726_223450.jpg";

  const images = [
    { image: img1, text: "Give me the treats!" },
    { image: img2, text: "Hello there" },
    { image: img3, text: "Welcome to my crib" },
    { image: img4, text: "Pet meeee" },
    { image: img5, text: "Are you comming?!" },
    { image: img6, text: "This is my spot" },
  ];

  export let index;
</script>

<div class="image-container">
  <picture class="img"
    ><img
      src={images[index].image}
      alt="Shiba inu dog"
    /></picture
  >
  <div class="text">{images[index].text}</div>
</div>

<style>
  .image-container {
    padding: 10px 0;
    background-color: white;
    border: solid white 5px;
    border-radius: 5px;
    display: grid;
    justify-items: center;
  }
  img {
      width: 600px;
      @media screen and (max-width: 600px) {
        width: 100%;
    }
 
  }
  .text {
    color: navy;
    font-family: "Playwrite CU", cursive;
    text-align: center;
    max-width: 90%;
  }
</style>
