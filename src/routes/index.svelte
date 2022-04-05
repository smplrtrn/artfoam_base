<script context="module">
  export const prerender = true;
</script>

<script>
</script>

<svelte:head>
  <title>art.foam</title>
</svelte:head>

<section>
  <h1>
    <div class="welcome">
      <picture>
        <source srcset="rdr-wlcm.webp" type="image/webp" />
        <img src="rdr-wlcm.png" alt="Welcome" />
      </picture>
    </div>
    new art foam.build
  </h1>
</section>

<style>
  section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    flex: 1;
  }

  h1 {
    width: 100%;
  }

  .welcome {
    position: relative;

    width: 100%;
    height: 0;
    padding: 0 0 calc(100% * 9 / 12) 0;
  }

  .welcome img {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    display: block;
  }
</style>
