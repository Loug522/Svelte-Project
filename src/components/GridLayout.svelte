<div class="container">
  <div class="box red">Red</div>
  <div class="box green">Green</div>
  <div class="box blue">Blue</div>
  <div class="box footer">Footer</div>
</div>

<style>
  .container {
    display: grid;
    grid-template-rows: repeat(4, 100px);
    grid-template-columns: repeat(4, 100px);
  }

  .red {
    background: #ee2c17;
    grid-area: 1 / 1 / 2 / 5; /* row-s column-s row-e column-e */
  }

  .green {
    background: #17ed2b;
    grid-row: 2 / span 2;
    grid-column: 1 / span 2;
  }

  .blue {
    background: #176dee;
    grid-row: 2 / 4;
    grid-column: 3 / -1;
  }

  .footer {
    background: rebeccapurple;
    grid-area: 4 / 1 / 6 / -1;
  }
</style>
