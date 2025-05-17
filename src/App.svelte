<script>
  import Header from "./components/Header.svelte";
  import Footer from "./components/Footer.svelte";
</script>

<main class="main-grid">
  <Header />
  <div class="hero">
    <h1>Hello, World!</h1>
  </div>
  <Footer />
</main>

<style>
  :global(#app, *) {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  main {
    width: 100vw;
  }

  .main-grid {
    display: grid;
    grid-template-rows: 1fr;
  }

  .hero {
    height: 85vh;
    align-content: center;
  }
</style>
