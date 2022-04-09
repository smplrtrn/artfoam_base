<script>
  import { page } from "$app/stores";
</script>

<footer>
  <nav class="m-links">
    <svg class="arr" viewBox="0 0 100 150">
      <polygon points="0,75 100,0 100,150 0,150" style="stroke-width:0" />
    </svg>
    <ul>
      <li class:active={$page.url.pathname === "/"}>
        <a sveltekit:prefetch href="/">Foam</a>
      </li>
      <li class:active={$page.url.pathname === "/notes"}>
        <a sveltekit:prefetch href="/notes">Notes</a>
      </li>
      <li class:active={$page.url.pathname === "/build"}>
        <a sveltekit:prefetch href="/build">Build</a>
      </li>
    </ul>
    <svg class="arr" viewBox="0 0 100 150">
      <polygon points="0,0 125,75 125,150 0,150" style="stroke-width:0" />
    </svg>
  </nav>
  <section id="footer">
    <nav class="f-links">
      <ul>
        <li><a sveltekit:prefetch href="/about">About art.foam</a></li>
        <li><a href="https://art.foam.io">Visit art.foam.io</a></li>
        <li><a sveltekit:prefetch href="/support">Get Help</a></li>
      </ul>
      <ul>
        <li><a sveltekit:prefetch href="/licence">Licence</a></li>
        <li><a sveltekit:prefetch href="/legal">Legal</a></li>
      </ul>
    </nav>
  </section>
</footer>

<style>
  footer {
    position: sticky;
    bottom: 0;
    display: flex;
    flex-direction: column;
    position: relative;
    width: 100%;
    padding: 1rem 0 0;
    height: 6rem;
  }

  footer nav.f-links {
    --background: var(--nav-bg);
    display: flex;
    justify-content: center;
    align-items: baseline;
    flex-direction: row;
    min-width: 98vw;
    max-width: 62ch;
  }

  footer nav.m-links {
    display: flex;
    justify-content: center;
    height: 4.5rem;
  }

  section#footer {
    background-color: var(--primary-color);
    background: linear-gradient(
      282deg,
      var(--primary-color) 72%,
      var(--auxiliary-color) 115%,
      var(--tertiary-color) 67.35%,
      var(--auxiliary-color) 23.45%,
      var(--tertiary-color) 119%
    );
    display: flex;
    justify-content: center;
  }

  svg.arr polygon {
    fill: var(--ltr-accent-color);
  }

  nav.m-links ul {
    position: relative;
    padding: 0 0.5rem;
    margin: 0;
    height: 4.5em;
    display: flex;
    justify-content: center;
    align-items: center;
    list-style: none;
    background: var(--tertiary-color);
  }

  nav.f-links ul {
    position: relative;
    padding: 0 0.5rem;
    margin: 0 auto;
    min-height: 4.5em;
    max-width: 69ch;
    display: flex;
    align-items: flex-start;
    list-style: none;
    font-weight: 400;
    flex-direction: column;
    justify-content: center;
  }

  .f-links ul li {
    max-width: 78ch;
  }

  .f-links a {
    font-size: 1rem;
    font-weight: 400;
  }

  li {
    position: relative;
    height: 100%;
  }

  li.active::before {
    --size: 5px;
    content: "";
    width: calc(var(--size) * 2);
    height: calc(var(--size) * 2);
    position: absolute;
    top: 0;
    left: calc(50% - var(--size));
    border-top: calc(var(--size) * 3) solid var(--dp-accent-color);
  }

  nav li a {
    display: flex;
    height: 100%;
    align-items: center;
    padding: 0 0.5rem;
    color: var(--heading-color);
    font-weight: 500;
    font-size: 1.1rem;
    text-transform: uppercase;
    letter-spacing: 0.1rem;
    text-decoration: none;
    transition: color 0.2s linear;
  }

  nav.f-links li a {
    text-transform: none;
  }

  a:hover {
    color: var(--accent-color);
  }
</style>
