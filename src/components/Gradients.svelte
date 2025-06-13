<div class="wrapper">
  <div class="box v1 v2 v3">
    <p>
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Reiciendis autem
      culpa optio natus quam ipsa voluptate temporibus saepe inventore atque.
    </p>
    <button class="btn">Lorem, ipsum dolor.</button>
  </div>
</div>

<style>
  .wrapper {
    display: flex;
    background-image: url("../assets/city.jpg");
    background-size: 500px 500px;
    background-color: #d27d22;
    width: 500px;
    height: 500px;
  }

  .box {
    --card-bg: #0d0a1a;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    margin: auto;
    height: 50%;
    width: 70%;
    border-radius: 1rem;
    /* background: hsl(255, 44%, 7%, 0.5); */
    background: hsl(
      from var(--card-bg) h s l / 0.3
    ); /* Not supported on all browsers yet */
    backdrop-filter: blur(5px);
  }

  .v3 {
    --border-width: 2px;
    position: relative;
    z-index: 1;

    ::before {
      content: "";
      position: absolute;
      z-index: -1;
      inset: 0; /* bottom, left, top, right */
      border: var(--border-width) solid transparent;
      border-radius: 1rem;
      background: linear-gradient(#18122f, #261e43);
      mask:
        linear-gradient(black, black) border-box,
        linear-gradient(black, black) padding-box;
      mask-composite: subtract;
    }
  }

  .v2 {
    z-index: 1;
    /* border: transparent 2px solid;
    background-color: #1c1634;
    background:
      radial-gradient(circle at 50% 150%, #18122f, #261e43) padding-box,
      linear-gradient(#18122f, #261e43) border-box; */
  }

  .v1 {
    z-index: 1;
    /* border: transparent 2px solid; 
    background-color: #1c1634;
     background-image: radial-gradient(circle at 50% 150%, #18122f, #18122f),
      linear-gradient(red, blue);
    background-origin: padding-box, border-box;
    background-clip: padding-box, border-box; */
  }

  p {
    margin: 1rem auto;
    height: 60%;
    width: 85%;
  }

  .btn {
    background-color: #0d0a1a;
    color: #ddd;
    font-size: 1em;
    font-weight: bold;
    border-radius: 1em;
    margin-inline: auto;
    padding: 1em 2em;
  }
</style>
