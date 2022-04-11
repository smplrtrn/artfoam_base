<script>
  import { page } from "$app/stores";
</script>

<header>
  <section id="header" />
  <section class="nav">
    <div class="tl-corner" />
    <!-- TODO put something else here? github link? -->
    <nav class="m-links">
      <svg class="arr" viewBox="0 0 100 150">
        <polygon points="0,0 100,0 100,150 0,75" style="stroke-width:0" />
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
        <polygon points="0,0 125,0 125,50 0,150" style="stroke-width:0" />
      </svg>
    </nav>

    <div class="tr-corner">
      <!-- TODO put something else here? github link? -->
    </div>
  </section>
</header>

<style>
  section#header {
    height: clamp(0.175rem, 0.185rem, 0.235rem);
    background-color: var(--frame-accent-color);
    background-size: cover;
  }

  section.nav {
    display: flex;
    justify-content: center;
  }

  .tl-corner,
  .tr-corner {
    width: 4.5rem;
    height: 4.5rem;
  }

  nav {
    display: flex;
    justify-content: center;
    height: 4.5rem;
  }

  svg.arr polygon {
    fill: var(--frame-accent-color);
  }

  ul {
    position: relative;
    padding: 0 0.5rem;
    margin: 0;
    height: 4.5em;
    display: flex;
    justify-content: center;
    align-items: center;
    list-style: none;
    background: var(--nav-bg);
  }

  li {
    position: relative;
    height: 100%;
    z-index: 1000;
  }

  li.active::before {
    --size: 5px;
    content: "";
    width: calc(var(--size) * 2);
    height: calc(var(--size) * 2);
    position: absolute;
    bottom: 0;
    left: calc(50% - var(--size));
    border-bottom: calc(var(--size) * 3) solid var(--dp-accent-color);
  }

  nav a {
    display: flex;
    height: 100%;
    align-items: center;
    padding: 0 clamp(0.1rem, 0.25rem, 0.5rem);
    color: var(--lt-text-color);
    font-weight: 500;
    font-size: clamp(1rem, 1.1rem, 1.2rem);
    text-transform: uppercase;
    letter-spacing: 0.135rem;
    text-decoration: none;
    transition: color 0.2s linear;
  }

  a:hover {
    color: var(--frame-accent-color);
  }
</style>
