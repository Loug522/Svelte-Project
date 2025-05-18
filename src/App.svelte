<script>
  import Header from "./components/Header.svelte";
  import Footer from "./components/Footer.svelte";
  import Main from "./components/Main.svelte";
  import SideArticles from "./components/SideArticles.svelte";
</script>

<main class="main-grid">
  <Header />
  <div class="main-container">
    <Main />
    <div class="sidebar">
      <SideArticles />
    </div>
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

  .main-container {
    display: flex;
    align-content: center;
    height: calc(100vh - 6.5rem);
  }
</style>
