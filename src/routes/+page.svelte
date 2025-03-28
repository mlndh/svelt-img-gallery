<script>
  // @ts-nocheck
  import Buttons from "./Buttons.svelte";
  import Images from "./Images.svelte";
  let index = 0;
</script>

<svelte:head>
  <title>Leon images</title>
  <meta name="description" content="Svelte demo app" />
</svelte:head>

<section class="container">
  <div class="images">
    <Images {index}></Images>
  </div>
  <Buttons bind:index></Buttons>
</section>

<style>
  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .images {
    min-height: 75vh;
    display: flex;
    align-items: center;
    @media screen and (max-width: 600px) {
      margin: 0 5px;
    }
  }
</style>
