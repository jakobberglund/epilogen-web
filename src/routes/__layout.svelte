<script lang="ts">
  import Header from '$lib/header/Header.svelte';
  import '../reset.css';
  import '../app.css';
</script>

<svelte:head>
  <link
    rel="stylesheet"
    href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond&display=swap"
  />
</svelte:head>

<div class="layout">
  <Header />
  <main>
    <slot />
  </main>
</div>

<style>
  .layout {
    min-height: 100vh;
    display: grid;
    grid-auto-flow: row;
    grid-template-rows: auto 1fr;
    align-items: center;
    text-align: center;
  }
</style>
