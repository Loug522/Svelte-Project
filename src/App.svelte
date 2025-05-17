<script>
  import Header from "./components/Header.svelte";
</script>

<main>
  <div class="wrapper">
    <Header />
    <h1>Hello, World!</h1>
  </div>
</main>

<style>
  * {
    box-sizing: border-box;
  }

  :global(body) {
    margin: 0;
    padding: 0;
  }

  .wrapper {
    width: 100vw;
  }
</style>
