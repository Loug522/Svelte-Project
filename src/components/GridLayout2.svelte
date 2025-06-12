<div class="container">
  <div class="box header">Header</div>
  <div class="box menu">Menu</div>
  <div class="box main">Main</div>
  <div class="box aside">Aside</div>
  <div class="box footer">Footer</div>
</div>

<style>
  .container {
    text-transform: uppercase;

    display: grid;
    grid-template-columns: 1fr 2fr 1fr;
    grid-template-rows: 1fr 5vh 3fr 5vh;
  }
</style>
