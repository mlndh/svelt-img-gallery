<script lang="ts">
  export let index = 0;
</script>

<div class="buttons-container">
  <button disabled={index <= 0} on:click={() => (index -= 1)} class="button"
    >Previous</button
  >

  <button disabled={index > 4} on:click={() => (index += 1)} class="button"
    >Next</button
  >
</div>

<style>
  .buttons-container {
    display: flex;
    gap: 20px;
    padding-top: 20px;
    @media screen and (max-width: 600px) {
      padding-top: 0px;
    }
  }

  .button {
    box-shadow:
      0 12px 16px 0 rgba(0, 0, 0, 0.24),
      0 17px 50px 0 rgba(0, 0, 0, 0.19);
    padding: 15px;
    border-radius: 10px;
    background-color: #e05115;
    color: #ffffff;
    letter-spacing: 2px;
    border: none;
    font-size: 21px;
    font-weight: bold;
    min-width: 200px;
    @media screen and (max-width: 600px) {
      font-size: 16px;
      padding: 10px;
      min-width: 150px;
    }
  }
  .button:hover {
    cursor: pointer;
    background-color: #da6327;
  }

  .button:disabled {
    cursor: auto;
    background-color: rgb(165, 158, 158);
  }
</style>
