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
    width: 500px;
    height: 500px;

    display: grid;
    grid-template-columns: 1fr 2fr 1fr;
    grid-template-rows: 10vh 1fr 3fr 10vh;
  }

  .header {
    grid-area: 1 / 1 / 2 / 5;
    background: red;
  }

  .main {
    grid-area: 2 / 1 / 3 / 5;
    background: goldenrod;
  }

  .menu {
    grid-area: 3 / 1 / 3 / 4;
    background: blue;
  }

  .aside {
    grid-area: 3 / 3 / 4 / 5;
    background: green;
  }

  .footer {
    grid-area: 4 / 1 / -1 / -1;
    background: purple;
  }
</style>
