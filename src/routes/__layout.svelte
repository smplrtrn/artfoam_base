<script>
  import Header from "$lib/header/Header.svelte";
  import Footer from "$lib/footer/Footer.svelte";
  import "../app.css";
</script>

<svelte:head>
  <link
    href="https://fonts.googleapis.com/css2?family=IBM+Plex+Sans&family=IBM+Plex+Serif:wght@300&display=swap"
    rel="stylesheet"
  />
  <link
    href="https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:ital,wght@0,300;1,300&display=swap"
    rel="stylesheet"
  />
</svelte:head>

<Header />

<main class="wrapper">
  <slot />
</main>

<Footer />

<style>
  main {
    flex: 1;
    display: flex;
    flex-direction: column;
    width: 100%;
    min-height: calc(100vh - 10rem);
    box-sizing: border-box;
  }
  .wrapper {
    width: clamp(16rem, 90vw, 70rem);
    margin-left: auto;
    margin-right: auto;
    padding-left: 0.5rem;
    padding-right: 0.5rem;
  }
</style>
