<script>
  import Header from "$lib/header/Header.svelte";
  import Footer from "$lib/footer/Footer.svelte";
  import "../app.css";
</script>

<svelte:head>
  <style>
    @import url("https://fonts.googleapis.com/css2?family=IBM+Plex+Mono:ital,wght@0,400;0,500;0,700;1,400&family=IBM+Plex+Sans:ital,wght@0,400;0,500;0,700;1,400&display=swap");
  </style>
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
    min-height: calc(
      100vh - 10rem - clamp(0.137rem, 0.145rem, 0.185rem) -
        clamp(0.137rem, 0.145rem, 0.185rem)
    );
    box-sizing: border-box;
  }
  .wrapper {
    width: clamp(16rem, 94vw, 72ch);
    margin-left: auto;
    margin-right: auto;
    padding-left: 0.5rem;
    padding-right: 0.5rem;
  }
</style>
