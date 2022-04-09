<script context="module">
  export const prerender = true;
</script>

<script>
</script>

<svelte:head>
  <title>art.foam.builder</title>
</svelte:head>

<div class="content">
  <h1>Foam</h1>
  <figure class="p-frame">
    <source srcset="qimg.webp" type="image/webp" />
    <filter
      id="filter"
      x="0%"
      y="0%"
      width="100%"
      height="100%"
      filterUnits="objectBoundingBox"
      primitiveUnits="userSpaceOnUse"
      color-interpolation-filters="sRGB"
    >
      <feColorMatrix
        type="matrix"
        values="1 0 0 0 0
            1 0 0 0 0
            1 0 0 0 0
            0 0 0 1 0"
        in="SourceGraphic"
        result="colormatrix"
      />
      <feComponentTransfer in="colormatrix" result="componentTransfer">
        <feFuncR type="table" tableValues="0.97 0.21 0.73" />
        <feFuncG type="table" tableValues="0.93 0.17 0.27" />
        <feFuncB type="table" tableValues="0.73 0.21 0.58" />
        <feFuncA type="table" tableValues="0 1" />
      </feComponentTransfer>
      <feBlend
        mode="multiply"
        in="componentTransfer"
        in2="SourceGraphic"
        result="blend"
      />
    </filter><img src="qimg.jpg" alt="Welcome" class="welcome" />
    <figcaption class="c-frame">What<br />else?</figcaption>
  </figure>
  <section class="t-frame">
    <article class="sheet">
      <h2>Well ...</h2>
      <p>
        apparently .... we'd need some more text to fill up the background. Wich
        would be absolutely fine, I think. Turns out it is not dynamicly
        adjusting, needs background-size set to cover. Maybe try contain
        instead?
      </p>
    </article>
  </section>
</div>

<style>
  .content {
    width: 100%;
    max-width: var(--column-width);
    margin: var(--column-margin-top) auto var(--column-margin-bottom) auto;
  }

  .t-frame {
    display: block;
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='100%25' height='100%25' viewBox='0 0 100 100'%3E%3Cg %3E%3Cpolygon fill='%238a8a8aef' points='0.42555,1.26458336 139.92594,1.8422832 286.61518,299.37616 -1.26458325,278.5873'/%3E%3C/g%3E%3C/svg%3E");
    background-size: cover;
    background-repeat: repeat;
    fill: var(--accent-color);
    width: auto;
    margin-left: auto;
    margin-right: auto;
    padding: clamp(0.349rem, 0.349vw, 0.849rem)
      clamp(0.1549rem, 0.4535vw, 0.649rem) clamp(0.1549rem, 0.1549vw, 0.49rem);
  }

  .sheet {
    display: flex;
    margin: 0.649rem 0.349rem 0.649rem;
    padding: 1rem;
    background: linear-gradient(
      209deg,
      var(--primary-color) 58%,
      var(--secondary-color) 201%,
      var(--tertiary-color) 32.35%,
      var(--secondary-color) 59.45%,
      var(--primary-color) -12%
    );
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'%3E%3Cg %3E%3Cpolygon fill='%23e9ebf0ea' points='1.02555,0.56458336 292.92594,-1.8422832 286.61518,289.37616 -3.26458325,288.5873'/%3E%3C/g%3E%3C/svg%3E");
    background-size: cover;
    flex-direction: column;
  }

  .p-frame {
    display: block;
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='100%25' height='100%25' viewBox='0 0 100 100'%3E%3Cg %3E%3Cpolygon fill='%238a8a8aef' points='1.02555,1.26458336 139.92594,1.8422832 286.61518,299.37616 -1.26458325,278.5873'/%3E%3C/g%3E%3C/svg%3E");
    background-size: cover;
    background-repeat: repeat;
    width: auto;
    margin-left: auto;
    margin-right: auto;
    padding-left: clamp(0.649rem, 1.349vw, 1.649rem);
    padding-right: clamp(0.349rem, 0.935vw, 1.349rem);
  }

  .c-frame {
    display: inline-flex;
    background: linear-gradient(
      209deg,
      var(--primary-color) 58%,
      var(--secondary-color) 201%,
      var(--tertiary-color) 32.35%,
      var(--secondary-color) 59.45%,
      var(--primary-color) -12%
    );
    background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 10'%3E%3Cg %3E%3Cpolygon fill='%23e9ebf0ea' points='-14.97445,0.56458336 292.92594,-1.842283 -4.38482,13.37616 -4.264583,12.5873'/%3E%3C/g%3E%3C/svg%3E");
    background-size: cover;
    background-repeat: no-repeat;
    color: var(--text-color);
    width: 49%;
    margin-left: 25%;
    margin-right: auto;
    padding: 0.5rem 0.5%;
    justify-content: space-evenly;
  }

  img.welcome {
    position: relative;
    filter: url(#filter);
    width: 100%;
    height: 100%;
  }
</style>
