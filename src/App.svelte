<script>
  import Gradients from "./components/Gradients.svelte";
  import GridLayout from "./components/GridLayout.svelte";
  import GridLayout2 from "./components/GridLayout2.svelte";
  import Inspecting from "./components/Inspecting-states.svelte";
</script>

<main>
  <div class="wrapper">
    <GridLayout2 />
    <Gradients />
  </div>

  <!-- <div class="card">
    <Inspecting />
  </div>
  <div class="box-container">
    <GridLayout />
  </div> -->
</main>

<style>
  .wrapper {
    display: inline flex;
    gap: 1rem;
  }
</style>
