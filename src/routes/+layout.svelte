<script>
  import "../app.css";
</script>

<div class="app">


  <main>
    <slot />
  </main>


</div>

<style>
  .app {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
    background-color: #15a4ea;
    font-size: 21px;
    padding: 10px;
    color: white;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  }
</style>
